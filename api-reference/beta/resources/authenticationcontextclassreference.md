---
title: тип ресурса authenticationContextClassReference
description: Представляет ссылку Azure Active Directory класса проверки подлинности.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1397545d7b102d05b8c71957cea88f9c131f0e09
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547534"
---
# <a name="authenticationcontextclassreference-resource-type"></a>тип ресурса authenticationContextClassReference

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ссылку Azure Active Directory класса проверки подлинности. Ссылки на класс контекста проверки подлинности — это настраиваемые значения, которые определяют требование проверки подлинности условного доступа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Проверка подлинности спискаContextClassReference](../api/conditionalaccessroot-list-authenticationcontextclassreferences.md) | [коллекция authenticationContextClassReference](authenticationContextClassReference.md) | Получите все объекты authenticationContextClassReference в организации. |
| [Создание проверки подлинностиContextClassReference](../api/conditionalaccessroot-post-authenticationcontextclassreferences.md) | [authenticationContextClassReference](authenticationContextClassReference.md) | Создание нового объекта проверки подлинностиContextClassReference. |
| [Проверка подлинностиContextClassReference](../api/authenticationcontextclassreference-get.md) | [authenticationContextClassReference](authenticationContextClassReference.md) | Чтение свойств и связей объекта authenticationContextClassReference. |
| [Обновление проверки подлинностиContextClassReference](../api/authenticationcontextclassreference-update.md) | [authenticationContextClassReference](authenticationContextClassReference.md) | Обновление объекта authenticationContextClassReference. |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Идентификатор, используемый для ссылки на класс контекста проверки подлинности. ID используется для запуска этапной проверки подлинности для ссылаемого требования к проверке подлинности и является значением, которое будет выдано в утверждении acrs. Это значение в утверждении используется для проверки удовлетворенности необходимого контекста проверки подлинности. Допустимые значения id — это "c1" через "c25". |
|displayName|String| Имя отображения — это удобное имя проверки подлинностиContextClassReference. Это значение следует использовать для определения ссылки класса контекста проверки подлинности при создании пользовательских интерфейсов администратора. Например, выбор UX. |
|description|String| Краткое объяснение политик, которые применяются при проверке подлинностиContextClassReference. Это значение следует использовать для предоставления дополнительного текста для описания ссылки класса контекста проверки подлинности при создании пользовательских интерфейсов администратора. Например, выбор UX.|
|isAvailable|boolean| Указывает, была ли проверка подлинностиContextClassReference опубликована администратором безопасности и готова к использованию приложениями. Если она установлена, ее не следует показывать в интерфейсе администрирования, так как в настоящее время значение не доступно `false` для выбора.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.authenticationContextClassReference",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id"
}-->

```json
    {
      "id": "String",
      "displayName": "String",
      "description": "String",
      "isAvailable": "boolean",
    }

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationContextClassReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
