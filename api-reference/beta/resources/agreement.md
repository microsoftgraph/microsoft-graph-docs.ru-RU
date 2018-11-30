---
title: Тип ресурса соглашения
description: Представляет клиента настраиваемый соглашение об условиях использования, который создается и управляется с помощью Azure Active Directory (Azure AD). Можно использовать следующие методы для создания и управления компонента Azure Active Directory условия использования согласно сценарию.
ms.openlocfilehash: 2e5c9087cd809f9c067150654d420fda533ca61b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077139"
---
# <a name="agreement-resource-type"></a>Тип ресурса соглашения

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет клиента настраиваемый соглашение об условиях использования, который создается и управляется с помощью Azure Active Directory (Azure AD). Можно использовать следующие методы для создания и управления [Azure Active Directory условия использования компонента](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) согласно сценарию.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание соглашения](../api/agreement-post-agreements.md) | [соглашения](agreement.md) | Создайте новое соглашение с учета в коллекцию соглашения. |
| [Соглашения по списку](../api/agreement-list.md) | [соглашение](agreement.md) семейства сайтов | Получение коллекции объектов соглашения. |
| [Получение соглашения](../api/agreement-get.md) | [соглашения](agreement.md) | Чтение свойства и связи объекта соглашения. |
| [Обновить соглашения](../api/agreement-update.md) | [соглашения](agreement.md) | Обновление объекта соглашения. |
| [Удаление соглашения](../api/agreement-delete.md) | Нет | Удаление объекта соглашения. |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String|Отображаемое имя соглашения.|
|id|String| Только для чтения.|
|isViewingBeforeAcceptanceRequired|Логический|Указывает, есть ли у пользователя можно развернуть и отобразить соглашения перед подтверждением.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|files|[agreementFile](agreementfile.md) коллекции|Только для чтения. PDF-файлы, связанные с этого соглашения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isViewingBeforeAcceptanceRequired": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
