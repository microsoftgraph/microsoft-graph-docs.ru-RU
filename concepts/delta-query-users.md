---
title: Получение добавочных изменений для пользователей
description: Запрос позволяет запрашивать добавления, удаления или обновления пользователей с помощью серии вызовов функции delta. Запрос изменений позволяет находить изменения пользователей. При этом не требуется получать полный набор пользователей из Microsoft Graph и сравнивать изменения.
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: be944c68d3c21fae5c1267cf95a7a926faaa2b355e6ea96dcb160b6f55107138
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180441"
---
# <a name="get-incremental-changes-for-users"></a>Получение добавочных изменений для пользователей

[Запрос](./delta-query-overview.md) позволяет запрашивать добавления, удаления или обновления пользователей с помощью серии вызовов функции [delta](/graph/api/user-delta?view=graph-rest-1.0). Запрос изменений позволяет находить изменения пользователей. При этом не требуется получать полный набор пользователей из Microsoft Graph и сравнивать изменения.

Клиенты, выполняющие синхронизацию пользователей с локальным хранилищем профилей, в ближайшем будущем смогут использовать запрос изменений как для первичной полной синхронизации, так и для добавочной синхронизации. Как правило, сначала выполняется полная синхронизация пользователей в клиенте, а потом периодически добавляются изменения.

## <a name="tracking-user-changes"></a>Отслеживание изменений пользователей

Как правило, цикл отслеживания изменений пользователей состоит из одного или нескольких запросов GET с вызовом функции **delta**. Запрос GET совершается практически так же, как и при [получении списка пользователей](/graph/api/user-list?view=graph-rest-1.0), но в него нужно включить:

- функцию **delta**;
- [маркер состояния](./delta-query-overview.md) (_deltaToken_ или _skipToken_) из данных предыдущего вызова функции **delta** в запросе GET.

## <a name="example"></a>Пример

В следующем примере показана серия запросов для отслеживания изменений пользователей:

1. [Исходный запрос](#initial-request) и [ответ](#initial-response)
2. [Запрос nextLink](#nextlink-request) и [ответ](#nextlink-response)
3. [Последний запрос nextLink](#final-nextlink-request) и [ответ](#final-nextlink-response)
4. [Запрос deltaLink ](#deltalink-request) и [ответ deltaLink](#deltalink-response)

## <a name="initial-request"></a>Исходный запрос

Чтобы начать отслеживать изменения в ресурсе пользователя, необходимо совершить к нему запрос, включающий функцию delta.

Обратите внимание на следующее:

- Необязательный параметр $select включен в запрос, чтобы продемонстрировать, как параметры запроса автоматически включаются в последующие запросы.
- Исходный запрос не включает маркер состояния. Маркеры состояния будут использоваться в последующих запросах.

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,givenName,surname
```

## <a name="initial-response"></a>Исходный ответ

В случае успеха этот метод возвращает код ответа `200 OK` и объект коллекции [user](/graph/api/resources/user?view=graph-rest-1.0) в тексте ответа. Если полный набор пользователей не помещается на одну страницу, ответ также будет включать маркер состояния nextLink.

В этом примере возвращается URL-адрес nextLink. Это означает, что в текущем сеансе можно получить дополнительные страницы данных. Параметр $select из исходного запроса кодируется в URL-адресе nextLink.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,givenName,surname)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa",
  "value": [
    {
      "displayName":"Testuser1",
      "givenName":"John",
      "surname":"Doe",
      "id":"ffff7b1a-13b6-477b-8c0c-380905cd99f7"
    },
    {
      "displayName":"Testuser2",
      "givenName":"Jane",
      "surname":"Doe",
      "id":"605d1257-ffff-40b6-8e6f-528a53f5dc55"
    }
  ]
}
```

## <a name="nextlink-request"></a>Запрос nextLink

Второй запрос указывает маркер `skipToken`, полученный из предыдущего ответа. Обратите внимание, что параметр `$select` указывать не обязательно, так как `skipToken` включает его в закодированном виде.

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa
```

## <a name="nextlink-response"></a>Ответ nextLink

Ответ содержит ссылку `nextLink` с новым значением `skipToken`, означающим, что доступны дополнительные группы. Вы должны продолжать выполнение запросов с использованием URL-адреса `nextLink`, пока в окончательном ответе не будет возвращен URL-адрес `deltaLink`, даже если значением является пустой массив (это может происходить при некоторых обстоятельствах).

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Testuser3",
      "givenName":"Pat",
      "surname":"Doe",
      "id":"d8c37826-ffff-4cae-b348-e2725b1e814b"
    },
    {
      "displayName":"Testuser4",
      "givenName":"Meghan",
      "surname":"Doe",
      "id":"8b1ee412-cd8f-4d59-ffff-24010edb9f1f"
    }
  ]
}
```

## <a name="final-nextlink-request"></a>Последний запрос nextLink

Третий запрос продолжает использовать маркер `skipToken`, полученный из последнего запроса на синхронизацию. 

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a>Последний ответ nextLink

Когда возвращается URL-адрес deltaLink, это означает, что больше нет данных о текущем состоянии ресурса. В последующих запросах приложение использует URL-адрес deltaLink, чтобы узнавать об изменениях ресурса. Сохраните маркер `deltaToken` и используйте его в URL-адресе запроса, чтобы находить изменения пользователей. 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Testuser5",
      "givenName":"Al",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "displayName":"Testuser6",
      "givenName":"Sam",
      "surname":"Doe",
      "id":"f6ede700-27d0-4c42-bfb9-4dffff43c74a"
    }
  ]
}
```

## <a name="deltalink-request"></a>Запрос deltaLink

С помощью маркера `deltaToken` из [последнего ответа](#final-nextlink-response) вы сможете получить пользователей, измененных (добавленных, удаленных или обновленных) с момента последнего запроса.

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460
```

## <a name="deltalink-response"></a>Ответ deltaLink

Если изменений не произошло, возвращается другой маркер `deltatoken` без результатов.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": []
}
```

Если же обнаружены изменения, возвращается другой маркер `deltatoken`, включающий коллекцию измененных пользователей.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": [
    {
      "displayName":"Testuser7",
      "givenName":"Joe",
      "surname":"Doe",
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

Ниже представлены некоторые примечания к предыдущему примеру отклика.

- Если пользователь удален, элемент содержит заметку: `@removed` со значением `"reason": "changed"`.

- Если пользователь удален окончательно, элемент содержит заметку: `@removed` со значением `"reason": "deleted"`.

- Заметок о создании или восстановлении пользователя не существует.

## <a name="see-also"></a>См. также
Обзор [запросов изменений Microsoft Graph](delta-query-overview.md).
