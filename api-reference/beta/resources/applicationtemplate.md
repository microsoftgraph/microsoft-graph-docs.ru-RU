---
title: Тип ресурса applicationTemplate
description: Представляет приложение в коллекции приложений Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c78834d027720371c1d259ce596fde82cb32ca46
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133212"
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
|description|Строка|Описание приложения.|
|displayName|Строка|Имя приложения.|
|homePageUrl|Строка|URL-адрес домашней страницы приложения.|
|id|Строка| Уникальный идентификатор приложения. Только для чтения.|
|logoUrl|Строка|URL-адрес для получения логотипа для этого приложения.|
|publisher|String|Имя издателя для этого приложения.|
|supportedProvisioningTypes|Коллекция объектов string|Список режимов предоставления, поддерживаемых этим приложением. Единственным допустимым значением `sync` является .|
|supportedSingleSignOnModes|Коллекция объектов string|Список режимов единого входов, поддерживаемых этим приложением. Поддерживаемые значения: `password`, `saml`, `external` и `oidc`.|

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



