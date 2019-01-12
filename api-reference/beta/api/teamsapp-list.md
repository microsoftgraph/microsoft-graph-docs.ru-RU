---
title: Список опубликованных приложений из каталога приложений группами Майкрософт
description: 'Список приложений из каталога приложений группами Майкрософт. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6f130d1842e8d860265adbdc82d8a5add9da025a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963698"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a>Список опубликованных приложений из каталога приложений группами Майкрософт

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Список [приложений](../resources/teamsapp.md) из каталога приложений группами Майкрософт. Этот компонент включает приложений из магазина группами Майкрософт, а также приложений из каталога приложений организации (каталог приложений клиента). Приобретать приложения в вашей организации только каталог приложений, укажите `Organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

>**Примечание:** Только глобальный администратор может вызывать этот интерфейс API. 

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)|
|:----------------------------------     |:-------------|
| Делегированные (рабочая или учебная учетная запись)     | AppCatalog.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается|
| Для приложений                            | Не поддерживается|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение           |
|:--------------|:--------------  |
| Авторизация | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Тело запроса
Нет.

>**Примечание:** Можно отфильтровать поля объекта [teamsCatalogApp](../resources/teamsapp.md) для сокращения списка результатов. Можно использовать любой из следующих операций фильтра: равно, не равно и, или, а не.

## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200 OK` код ответа и список объектов [teamsCatalogApp](../resources/teamsapp.md) в теле ответа.

## <a name="examples"></a>Примеры
### <a name="example-1"></a>Пример 1
В следующем примере перечисляются все приложения, которые специфичны для вашего клиента.

#### <a name="request"></a>Запрос
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a>Ответ
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

### <a name="example-2"></a>Пример 2

В следующем примере перечисляются приложений с указанным идентификатором.

#### <a name="request"></a>Запрос
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a>Ответ
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

