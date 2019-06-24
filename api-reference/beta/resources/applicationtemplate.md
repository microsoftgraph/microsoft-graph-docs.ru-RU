---
title: Тип ресурса Аппликатионтемплате
description: Представляет приложение в коллекции приложений Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a8e1f4cb365f86df32e32ed568aa3a96d1c090f
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147937"
---
# <a name="applicationtemplate-resource-type"></a>Тип ресурса Аппликатионтемплате

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет приложение в [коллекции приложений Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/saas-apps/tutorial-list).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Список Аппликатионтемплате](../api/applicationtemplate-list.md)|[Аппликатионтемплате](applicationtemplate.md)|Получение списка объектов Аппликатионтемплате.|
| [Получение Аппликатионтемплате](../api/applicationtemplate-get.md) | [Аппликатионтемплате](applicationtemplate.md) | Чтение свойств и связей объекта Аппликатионтемплате. |
|[Создание экземпляра Аппликатионтемплате](../api/applicationtemplate-instantiate.md)|[АппликатионсервицепринЦипал](applicationserviceprincipal.md)| Добавьте экземпляр приложения из коллекции приложений Azure AD в ваш каталог.|


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|categories|Коллекция String|Список категорий для приложения. Допустимые `Collaboration`значения:, `Business Management`, `Consumer`,`Content management` `CRM` `Data services` `Developer services` `E-commerce` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Human resources` `Finance` `Health`,,,,,,,,,,,,,,,,,,,, `Education` `ERP` , `Project management`, `Telecommunications`, `Tools, Travel`, и `Web design & hosting`.|
|description|String|Описание приложения.|
|displayName|Строка|Имя приложения.|
|Хомепажеурл|String|URL-адрес домашней страницы приложения.|
|id|Строка| Уникальный идентификатор приложения. Только для чтения.|
|logoUrl|String|URL-адрес для получения логотипа для этого приложения.|
|publisher|String|Имя издателя для этого приложения.|
|Суппортедпровисионингтипес|Коллекция строк|Список режимов подготовки, поддерживаемых этим приложением. Единственное допустимое значение: `sync`.|
|Суппортедсинглесигнонмодес|Коллекция строк|Список режимов единого входа, поддерживаемых этим приложением. `password`Поддерживаемые значения: `saml`, `external`, и. `oidc`|

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
