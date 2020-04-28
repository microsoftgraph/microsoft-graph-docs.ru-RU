---
title: Тип ресурса договора
description: Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 6ac24e7a46441b59e621425517371db9227b4010
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218487"
---
# <a name="agreement-resource-type"></a>Тип ресурса договора

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD). Вы можете использовать следующие методы для создания и управления [условиями использования функции Azure Active Directory](/azure/active-directory/active-directory-tou) в соответствии со сценарием.

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
|displayName|Строка|Отображаемое имя соглашения.|
|id|String| Только для чтения.|
|исвиевингбефореакцептанцерекуиред|Boolean|Указывает, должно ли пользователь развернуть и просмотреть Соглашение перед принятием.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
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
