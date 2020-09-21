---
title: Тип ресурса Аппликатионтемплате
description: Представляет приложение в коллекции приложений Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1dcb5d1a4f1a86521081487ec66494d76c035b82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050236"
---
# <a name="applicationtemplate-resource-type"></a>Тип ресурса Аппликатионтемплате

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет приложение в [коллекции приложений Azure AD](/azure/active-directory/saas-apps/tutorial-list).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Перечисление applicationTemplate](../api/applicationtemplate-list.md)|[applicationTemplate](applicationtemplate.md)|Получение списка объектов Аппликатионтемплате.|
| [Получение Аппликатионтемплате](../api/applicationtemplate-get.md) | [applicationTemplate](applicationtemplate.md) | Чтение свойств и связей объекта Аппликатионтемплате. |
|[Создание экземпляра applicationTemplate](../api/applicationtemplate-instantiate.md)|[аппликатионсервицепринЦипал](applicationserviceprincipal.md)| Добавьте экземпляр приложения из коллекции приложений Azure AD в ваш каталог.|


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|categories|Коллекция String|Список категорий для приложения. Поддерживаются следующие значения:,,,,,,,,,, `Collaboration` `Business Management` `Consumer` `Content management` `CRM` `Data services` `Developer services` `E-commerce` `Education` `ERP` `Finance` `Health` , `Human resources` , `IT infrastructure` , `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools, Travel` `Web design & hosting` ,,,,,,,,,,,,,, и.|
|description|String|Описание приложения.|
|displayName|Строка|Имя приложения.|
|хомепажеурл|Строка|URL-адрес домашней страницы приложения.|
|id|Строка| Уникальный идентификатор приложения. Только для чтения.|
|logoUrl|Строка|URL-адрес для получения логотипа для этого приложения.|
|publisher|String|Имя издателя для этого приложения.|
|суппортедпровисионингтипес|Коллекция String|Список режимов подготовки, поддерживаемых этим приложением. Единственное допустимое значение: `sync` .|
|суппортедсинглесигнонмодес|Коллекция String|Список режимов единого входа, поддерживаемых этим приложением. Поддерживаемые значения: `password` ,, `saml` `external` и `oidc` .|

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


