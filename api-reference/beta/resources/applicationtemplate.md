---
title: Тип ресурса Аппликатионтемплате
description: Представляет приложение в коллекции приложений Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0c34c083a4cfee63db724228d9390c7452ca5a92
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870948"
---
# <a name="applicationtemplate-resource-type"></a>Тип ресурса Аппликатионтемплате

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет приложение в [коллекции приложений Azure AD](/azure/active-directory/saas-apps/tutorial-list).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Список Аппликатионтемплате](../api/applicationtemplate-list.md)|[аппликатионтемплате](applicationtemplate.md)|Получение списка объектов Аппликатионтемплате.|
| [Получение Аппликатионтемплате](../api/applicationtemplate-get.md) | [аппликатионтемплате](applicationtemplate.md) | Чтение свойств и связей объекта Аппликатионтемплате. |
|[Создание экземпляра Аппликатионтемплате](../api/applicationtemplate-instantiate.md)|[аппликатионсервицепринЦипал](applicationserviceprincipal.md)| Добавьте экземпляр приложения из коллекции приложений Azure AD в ваш каталог.|


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|categories|Коллекция String|Список категорий для приложения. Поддерживаются следующие значения: `Collaboration`, `Business Management`, `Consumer`,`Content management` `CRM` `Data services` `Developer services` `E-commerce` `Education` `Health` `Human resources` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Web design & hosting`,,,,,,,,, `Tools, Travel`, `Telecommunications`,,,,,,,,,,,,,, и. `Project management` `ERP` `Finance`|
|description|String|Описание приложения.|
|displayName|Строка|Имя приложения.|
|хомепажеурл|String|URL-адрес домашней страницы приложения.|
|id|Строка| Уникальный идентификатор приложения. Только для чтения.|
|logoUrl|String|URL-адрес для получения логотипа для этого приложения.|
|publisher|String|Имя издателя для этого приложения.|
|суппортедпровисионингтипес|Коллекция строк|Список режимов подготовки, поддерживаемых этим приложением. Единственное допустимое значение: `sync`.|
|суппортедсинглесигнонмодес|Коллекция строк|Список режимов единого входа, поддерживаемых этим приложением. `password`Поддерживаемые значения: `saml`, `external`, и. `oidc`|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
