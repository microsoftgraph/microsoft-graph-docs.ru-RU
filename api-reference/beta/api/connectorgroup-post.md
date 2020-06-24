---
title: Создание Коннекторграуп
description: Создание объекта Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ddc1aebfeb64e4dd596f94dd8a91f3718a29fb7
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863274"
---
# <a name="create-connectorgroup"></a>Создание Коннекторграуп

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание объекта [коннекторграуп](../resources/connectorgroup.md) .

## <a name="permissions"></a>Разрешения
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается.  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-request-headers"></a>Необязательные заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Носителя. Обязательный параметр.|
| Content-Type | application/json. Required. |

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [коннекторграуп](../resources/connectorgroup.md) в формате JSON.
В следующей таблице перечислены свойства, доступные для **коннекторграуп**. Свойство **Name** — это обязательное свойство.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|коннекторграуптипе|string| Указывает тип гибридного агента. Это свойство предустановлено системой.|
|id|строка| Уникальный идентификатор для этого Коннекторграуп. Только для чтения. |
|isDefault|boolean| Указывает, является ли Коннекторграуп значением по умолчанию. Только одна группа соединителей может быть Коннекторграуп по умолчанию, и она предустановлена системой. |
|name|string| Имя, связанное с Коннекторграуп. |
|региональных|string| Регион, которому назначена Коннекторграуп, и который оптимизирует трафик для. Эту область можно задать только в том случае, если Коннекторграуп **не назначен ни один** из соединителей или приложений. Доступны следующие регионы: Северная Америка, Европа, Австралия, Азия и Индии. Возможные значения: `nam`, `eur`, `aus`, `asia`, `ind`.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [коннекторграуп](../resources/connectorgroup.md) в тексте отклика.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "Connector Group Demo"

}
```
### <a name="response"></a>Отклик
Ниже приведен пример отклика. 

>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "3e6f4c35-a04b-4d03-b98a-66fff89b72e6",
  "name": "Connector Group Demo",
  "connectorGroupType": "applicationProxy",
  "isDefault": true,
  "region": "nam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
