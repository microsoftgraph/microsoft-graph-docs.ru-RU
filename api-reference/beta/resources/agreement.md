---
title: Тип ресурса договора
description: Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD). Вы можете использовать следующие методы для создания и управления условиями использования функции Azure Active Directory в соответствии со сценарием.
localization_priority: Normal
ms.openlocfilehash: d91cc8f8180ffb706639fb42a8c68d711991602c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339176"
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

## <a name="relationships"></a>Отношения
| Отношение | Тип        | Описание |
|:-------------|:------------|:------------|
|files|Коллекция [агриментфиле](agreementfile.md)|Только для чтения. Документы PDF, связанные с этим соглашением.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "suppressions": []
}
-->
