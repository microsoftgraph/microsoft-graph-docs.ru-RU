---
title: Тип ресурса applicationTemplate
description: Представляет приложение в коллекции приложений Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 37468877721b9ac534c0118aeb93fd613fca7f88
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159180"
---
# <a name="applicationtemplate-resource-type"></a>Тип ресурса applicationTemplate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет приложение в коллекции [приложений Azure AD.](/azure/active-directory/saas-apps/tutorial-list)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Перечисление applicationTemplate](../api/applicationtemplate-list.md)|[applicationTemplate](applicationtemplate.md)|Получение списка объектов applicationTemplate.|
| [Получение applicationTemplate](../api/applicationtemplate-get.md) | [applicationTemplate](applicationtemplate.md) | Чтение свойств и связей объекта applicationTemplate. |
|[Создание экземпляра applicationTemplate](../api/applicationtemplate-instantiate.md)|[applicationServicePrincipal](applicationserviceprincipal.md)| Добавьте экземпляр приложения из коллекции приложений Azure AD в каталог.|


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|categories|Коллекция String|Список категорий для приложения. Поддерживаемые значения: `Collaboration` , , , , `Business Management` `Consumer` , `Content management` , , `CRM` , , `Data services` , `Developer services` `E-commerce` `Education` `ERP` `Finance` `Health` `Human resources` и `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools, Travel` `Web design & hosting` .|
|description|String|Описание приложения.|
|displayName|String|Имя приложения.|
|homePageUrl|String|URL-адрес домашней страницы приложения.|
|id|String| Уникальный идентификатор приложения. Только для чтения.|
|logoUrl|String|URL-адрес для получения логотипа для этого приложения.|
|publisher|String|Имя издателя для этого приложения.|
|supportedProvisioningTypes|Коллекция String|Список режимов предоставления, поддерживаемых этим приложением. Единственным допустимым значением `sync` является .|
|supportedSingleSignOnModes|Коллекция String|Список режимов единого входов, поддерживаемых этим приложением. Поддерживаемые значения: `password`, `saml`, `external` и `oidc`.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
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



