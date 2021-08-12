---
title: тип ресурса applicationTemplate
description: Представляет приложение в галерее приложений Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: f9ec36c667bdf4e253b0b8bcc555e77bf7659e554a115f1f7ec39b7b22f3f8f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155199"
---
# <a name="applicationtemplate-resource-type"></a>тип ресурса applicationTemplate

Пространство имен: microsoft.graph

Представляет приложение в галерее [приложений Azure AD.](/azure/active-directory/saas-apps/tutorial-list)

## <a name="methods"></a>Методы

| Метод                                                                       | Возвращаемый тип                                                   | Описание                                                                                  |
| :--------------------------------------------------------------------------- | :------------------------------------------------------------ | :------------------------------------------------------------------------------------------- |
| [Перечисление applicationTemplate](../api/applicationtemplate-list.md)               | [applicationTemplate](applicationtemplate.md)                 | Получение списка объектов applicationTemplate.                                              |
| [Получение applicationTemplate](../api/applicationtemplate-get.md)                 | [applicationTemplate](applicationtemplate.md)                 | Чтение свойств и связей объекта applicationTemplate.                             |
| [Создание экземпляра applicationTemplate](../api/applicationtemplate-instantiate.md) | [applicationServicePrincipal](applicationserviceprincipal.md) | Добавьте экземпляр приложения из галереи приложений Azure AD в каталог. |

## <a name="properties"></a>Свойства

| Свойство                   | Тип              | Описание                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| :------------------------- | :---------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| categories                 | Коллекция String | Список категорий для приложения. Поддерживаемые значения могут быть: `Collaboration` `Business Management` , `Consumer` `Content management` `CRM` `Data services` `Developer services` `E-commerce` `Education` `ERP` `Finance` , и `Health` `Human resources` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools` `Travel` `Web design & hosting` . |
| description                | String            | Описание приложения.                                                                                                                                                                                                                                                                                                                                                                                                               |
| displayName                | String            | Имя приложения.                                                                                                                                                                                                                                                                                                                                                                                                                    |
| homePageUrl                | String            | URL-адрес домашней страницы приложения.                                                                                                                                                                                                                                                                                                                                                                                                           |
| id                         | String            | Уникальный идентификатор для приложения. Только для чтения.                                                                                                                                                                                                                                                                                                                                                                                               |
| logoUrl                    | String            | URL-адрес для получения логотипа для этого приложения.                                                                                                                                                                                                                                                                                                                                                                                                   |
| publisher                  | String            | Имя издателя для этого приложения.                                                                                                                                                                                                                                                                                                                                                                                                 |
| supportedProvisioningTypes | Коллекция строк | Список режимов подготовка, поддерживаемых этим приложением. Единственным допустимым значением `sync` является .                                                                                                                                                                                                                                                                                                                                                   |
| supportedSingleSignOnModes | Коллекция String | Список режимов единой регистрации, поддерживаемых этим приложением. Поддерживаемые значения: `oidc`, `password`, `saml` и `notSupported`.                                                                                                                                                                                                                                                                                                            |

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
  "id": "id-value",
  "displayName": "displayName-value",
  "homePageUrl": "homePageUrl-value",
  "supportedSingleSignOnModes": ["supportedSingleSignOnModes-value"],
  "logoUrl": "logoUrl-value",
  "categories": ["categories-value"],
  "publisher": "publisher-value",
  "description": "description-value"
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
