---
title: Тип ресурса договора
description: Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD). Вы можете использовать следующие методы для создания и управления условиями использования функции Azure Active Directory в соответствии со сценарием.
localization_priority: Normal
ms.openlocfilehash: b253877f1bf82e4fbc61cebaef3c1bce208d9cca
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535750"
---
# <a name="agreement-resource-type"></a>Тип ресурса договора

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD). Вы можете использовать следующие методы для создания и управления [условиями использования функции Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) в соответствии со сценарием.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание договоров](../api/agreement-post-agreements.md) | [Корпоратив](agreement.md) | Создание нового соглашения путем публикации в коллекции договоров. |
| [Список соглашений](../api/agreement-list.md) | Коллекция [договоров](agreement.md) | Получение коллекции объектов Agreement. |
| [Получение соглашения](../api/agreement-get.md) | [Корпоратив](agreement.md) | Чтение свойств и связей объекта Agreement. |
| [Обновление соглашения](../api/agreement-update.md) | [Корпоратив](agreement.md) | Обновление объекта договора. |
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
|Исвиевингбефореакцептанцерекуиред|Логический|Указывает, должно ли пользователь развернуть и просмотреть Соглашение перед принятием.|

## <a name="relationships"></a>Связи
| Отношение | Тип        | Описание |
|:-------------|:------------|:------------|
|files|Коллекция [агриментфиле](agreementfile.md)|Только для чтения. Документы PDF, связанные с этим соглашением.|

## <a name="json-representation"></a>Представление в формате JSON

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
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreement.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
