---
title: Тип ресурса Аппликатионтемплате
description: Представляет приложение в коллекции приложений Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c707a9010103f4226e62782a83891ff880a245e8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508263"
---
# <a name="applicationtemplate-resource-type"></a>Тип ресурса Аппликатионтемплате

Пространство имен: microsoft.graph

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
|суппортедпровисионингтипес|Коллекция объектов string|Список режимов подготовки, поддерживаемых этим приложением. Единственное допустимое значение: `sync`.|
|суппортедсинглесигнонмодес|Коллекция объектов string|Список режимов единого входа, поддерживаемых этим приложением. `password`Поддерживаемые значения: `saml`, `external`, и. `oidc`|

## <a name="relationships"></a>Связи

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
