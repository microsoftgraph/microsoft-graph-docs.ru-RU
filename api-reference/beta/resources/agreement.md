---
title: Тип ресурса договора
description: Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 8b5b400bea6ae4435e1aa525012b7b3224a95abc
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2020
ms.locfileid: "49555653"
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
|displayName|String|Отображаемое имя соглашения. Отображаемое имя используется для внутренней трассировки соглашения, но оно не отображается для конечных пользователей, которые просматривают соглашение.|
|id|String| Только для чтения.|
|isPerDeviceAcceptanceRequired|Логический|Этот параметр позволяет конечным пользователям принимать данное соглашение для всех устройств, к которым они обращаются. Конечному пользователю потребуется зарегистрировать свое устройство в Azure AD, если это еще не сделано.|
|исвиевингбефореакцептанцерекуиред|Логический|Указывает, должно ли пользователь расширить Соглашение перед принятием.|
|termsExpiration|[termsExpiration](termsexpiration.md)| Расписание истечения срока действия и периодичность соглашения для всех пользователей. |
|userReacceptRequiredFrequency|Длительность|Срок действия, по истечении которого пользователь должен повторно принять условия использования. Значение представляется в формате ISO 8601 для длительности.|


## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|приемы|Коллекция [agreementAcceptance](agreementacceptance.md)|Только для чтения. Сведения о приемках настоящего соглашения.|
|files|Коллекция [агриментфилелокализатион](agreementfilelocalization.md)| Документы PDF, связанные с этим соглашением. **Примечание:** Это свойство является устаревшим. Вместо этого используйте свойство  **File** .|
|file|[agreementFile](agreementfile.md) | PDF-файл по умолчанию, связанный с этим соглашением.|
|файлы и локализации|Коллекция [агриментфилелокализатион](agreementfilelocalization.md)|Локализованные версии файлов соглашений, вложенных в соглашение.|
|файл/локализация/{Локализатионид}/версии|Коллекция [агриментфилеверсион](agreementfileversion.md)|Журнал версий для файла локализованного соглашения.|


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
  "id": "String (identifier)",
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "isPerDeviceAcceptanceRequired": false,
  "termsExpiration": {
    "startDateTime": "2018-10-01T00:00:00.0000000Z",
    "frequency": "PT1M"
  }
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


