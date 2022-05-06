---
title: Получение добавочных изменений для пользователей
description: Разностный запрос в Microsoft Graph позволяет запрашивать добавления, удаления или обновления поддерживаемых ресурсов. Он включается с помощью серии разностных запросов. Для пользователей разностный запрос позволяет обнаруживать изменения, не извлекая весь набор пользователей для сравнения изменений.
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: d03762372a789d76d3f38121da47d662e281b2f2
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247226"
---
# <a name="get-incremental-changes-for-users"></a>Получение добавочных изменений для пользователей

[Разностный запрос](./delta-query-overview.md) в Microsoft Graph позволяет запрашивать добавления, удаления или обновления [поддерживаемых ресурсов](delta-query-overview.md#supported-resources). Он включается с помощью серии [разностных](/graph/api/user-delta) запросов. Для пользователей разностный запрос позволяет обнаруживать изменения, не извлекая весь набор пользователей для сравнения изменений.

Клиенты, синхронизирующие пользователей с локальным хранилищем профилей, могут использовать дельта-запрос для первоначальной полной синхронизации, а также для последующих добавочных синхронизаций. Как правило, клиент выполняет первоначальную полную синхронизацию всех пользователей в клиенте, а затем периодически вносит добавочные изменения в пользователей.

## <a name="track-changes-to-users"></a>Отслеживание изменений пользователей

Отслеживайте изменения пользователей с помощью одного или нескольких запросов GET с помощью функции **delta**. Запрос GET похож на запрос [перечисления пользователей](/graph/api/user-list), за исключением следующих дополнительных объектов в URL.

- функцию **delta**;
- [маркер состояния](./delta-query-overview.md) (_deltaToken_ или _skipToken_) из данных предыдущего вызова функции **delta** в запросе GET.

## <a name="example-to-track-changes-to-users"></a>Пример отслеживания изменений пользователей

В следующем примере показана серия запросов для отслеживания изменений пользователей.

1. [Исходный запрос](#initial-request) и [отклик](#initial-response)
2. [Запрос nextLink](#nextlink-request) и [отклик](#nextlink-response)
3. [Последний запрос nextLink](#final-nextlink-request) и [отклик](#final-nextlink-response)
4. [Запрос deltaLink ](#deltalink-request) и [отклик deltaLink](#deltalink-response)

Обратите внимание на следующее в откликах.

- Если пользователь удален, элемент содержит заметку: `@removed` со значением `"reason": "changed"`.
- Если пользователь удален окончательно, элемент содержит заметку `@removed` со значением `"reason": "deleted"`.
- Заметок о создании или восстановлении пользователя не существует.

### <a name="initial-request"></a>Исходный запрос

Чтобы отслеживать изменения в ресурсе пользователя, создайте запрос и включите функцию **delta** в виде сегмента URL-адреса.

Обратите внимание на следующие элементы.

- Необязательный параметр `$select` включен в запрос, чтобы продемонстрировать, как параметры запроса автоматически включаются в последующие запросы.
- Первоначальный запрос не включает токен состояния. Токены состояния будут использоваться в последующих запросах.

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,givenName,surname
```

### <a name="initial-response"></a>Исходный отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект [пользовательской](/graph/api/resources/user) коллекции в тексте отклика. Предполагая, что полный набор пользователей слишком велик, отклик также будет включать токен состояния `@odata.nextLink` в параметре `@odata.nextLink`.

В этом примере возвращается URL-адрес `@odata.nextLink`, указывающий, что в сеансе есть дополнительные страницы данных для извлечения. Параметр `$select` исходного запроса закодирован в URL-адресе `@odata.nextLink`.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,givenName,surname)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa",
  "value": [
    {
      "displayName":"Cameron White",
      "givenName":"Cameron",
      "surname":"White",
      "id":"ffff7b1a-13b6-477b-8c0c-380905cd99f7"
    },
    {
      "displayName":"Delia Dennis",
      "givenName":"Delia",
      "surname":"Dennis",
      "id":"605d1257-ffff-40b6-8e6f-528a53f5dc55"
    },
    {
      "id": "86462606-fde0-4fc4-9e0c-a20eb73e54c6",
      "@removed": {
        "reason": "deleted"
      }
    },
    {
      "displayName": "Conf Room Adams",
      "id": "6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0"
    }
  ]
}
```

### <a name="nextlink-request"></a>Запрос nextLink

Второй запрос указывает `skipToken`, возвращенный предыдущим откликом. Обратите внимание, что параметр `$select` закодирован и включен в `skipToken`.

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa
```

### <a name="nextlink-response"></a>Отклик nextLink

Отклик содержит другой объект `@odata.nextLink` с новым значением `skipToken`, означающим, что доступны дополнительные изменения, которые были отслежены для пользователей. Используйте URL-адрес `@odata.nextLink` в других запросах, пока URL-адрес `@odata.deltaLink` (в параметре `@odata.deltaLink`) не будет возвращен в окончательном отклике, даже если значение является пустым массивом.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Mallory Cortez",
      "givenName":"Mallory",
      "surname":"Cortez",
      "id":"d8c37826-ffff-4cae-b348-e2725b1e814b"
    },
    {
      "displayName":"Diego Sicilian",
      "givenName":"Diego",
      "surname":"Sicilian",
      "id":"8b1ee412-cd8f-4d59-ffff-24010edb9f1f"
    }
  ]
}
```

### <a name="final-nextlink-request"></a>Последний запрос nextLink

Третий запрос использует последний `skipToken`, полученный из последнего запроса на синхронизацию. 

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

### <a name="final-nextlink-response"></a>Последний отклик nextLink

URL-адрес `@odata.deltaLink` возвращается, когда больше нет данных о существующем состоянии пользовательских объектов. Для будущих запросов приложение использует URL-адрес `@odata.deltaLink`, чтобы узнать об изменениях других пользователей. Сохраните `deltaToken` и используйте его в следующем URL-адресе запроса, чтобы узнать больше об изменениях для пользователей.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Lidia Holloway",
      "givenName":"Lidia",
      "surname":"Holloway",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "displayName":"Patti Fernandez",
      "givenName":"Patti",
      "surname":"Fernandez",
      "id":"f6ede700-27d0-4c42-bfb9-4dffff43c74a"
    }
  ]
}
```

### <a name="deltalink-request"></a>Запрос deltaLink

С помощью параметра `deltaToken` из [последнего отклика](#final-nextlink-response) вы сможете получить изменения (добавления, удаления или обновления) пользователей с момента последнего запроса.

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460
```

## <a name="deltalink-response"></a>Отклик deltaLink

Если изменений не произошло, возвращается объект `@odata.deltaLink` без результатов (свойство **value** является пустым массивом).

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": []
}
```

Если обнаружены изменения, в отклик включается коллекция измененных объектов user. Отклик также содержит ссылку `@odata.nextLink` (если требуется получить несколько страниц) или `@odata.deltaLink`. Реализуйте такой же порядок перехода по объектам `@odata.nextLink`, сохраняя заключительный объект `@odata.deltaLink` для последующих вызовов.

>**Примечание.** При запросе могут происходить задержки репликации для пользователей, которые были недавно созданы, обновлены или удалены. Повторите `@odata.nextLink` или `@odata.deltaLink` через некоторое время, чтобы получить последние изменения.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": [
    {
      "displayName":"MOD Administrator",
      "givenName":"MOD",
      "surname":"Administrator",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "id":"8ffff70c-1c63-4860-b963-e34ec660931d",
      "@removed": {
         "reason": "changed"
      }
    }
  ]
}
```

## <a name="see-also"></a>См. также
+ Обзор [запросов изменений Microsoft Graph](delta-query-overview.md).
