---
title: тип ресурса соглашения
description: Представляет настраиваемые условия соглашения об использовании клиента, которое создается и управляется с Azure Active Directory (Azure AD).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 21563f8a0c884c1b290a4dad8c807e7b2e9d3e81
ms.sourcegitcommit: 9759b647acfbed99d5675a6f512aaa33932a723f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/23/2021
ms.locfileid: "61604401"
---
# <a name="agreement-resource-type"></a>тип ресурса соглашения

Пространство имен: microsoft.graph

Представляет настраиваемые условия соглашения об использовании клиента, которое создается и управляется с Azure Active Directory (Azure AD). Вы можете использовать следующие методы для создания и управления функцией [Azure Active Directory терминов использования](/azure/active-directory/conditional-access/terms-of-use) в соответствии с вашим сценарием.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список соглашений](../api/agreement-list.md) | [коллекция соглашений](agreement.md) | Получите коллекцию объектов соглашения. |
| [Создание соглашений](../api/agreement-post-agreements.md) | [соглашение](agreement.md) | Создайте новое соглашение, разместив в коллекции соглашений. |
| [Получение соглашения](../api/agreement-get.md) | [соглашение](agreement.md) | Чтение свойств и связей объекта соглашения. |
| [Обновление соглашения](../api/agreement-update.md) | [соглашение](agreement.md) | Обновление объекта соглашения. |
| [Удаление соглашения](../api/agreement-delete.md) | Нет | Удаление объекта соглашения. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|Строка|Отображение имени соглашения. Имя отображения используется для внутреннего отслеживания соглашения, но не отображается конечным пользователям, которые просматривают соглашение.|
|id|Строка| Идентификатор соглашения. Только для чтения.|
|isPerDeviceAcceptanceRequired|Boolean|Указывает, должны ли конечные пользователи принимать это соглашение на каждом устройстве, с которое они имеют к нему доступ. Конечный пользователь должен зарегистрировать свое устройство в Azure AD, если он еще этого не сделал.|
|isViewingBeforeAcceptanceRequired|Boolean|Указывает, должен ли пользователь расширить соглашение перед принятием.|
|termsExpiration|[termsExpiration](termsexpiration.md)| Срок действия и периодичность соглашения для всех пользователей. |
|userReacceptRequiredFrequency|Длительность|Продолжительность, после которой пользователь должен повторно принять условия использования. Значение представлено в формате ISO 8601 для длительности.|


## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|приемки|Коллекция [agreementAcceptance](agreementacceptance.md)|Только для чтения. Сведения о принятии этого соглашения.|
|files|[коллекция agreementFileLocalization](agreementfilelocalization.md)| PDF, связанные с этим соглашением. Это свойство находится в процессе сноса. Вместо этого  **используйте свойство** file.|
|file|[agreementFile](agreementfile.md) | PDF по умолчанию, связанный с этим соглашением.|
|локализация|[коллекция agreementFileLocalization](agreementfilelocalization.md)|Локализованные версии файлов соглашений, присоединенных к соглашению.|
|versions|[коллекция agreementFileVersion](agreementfileversion.md)|История версий для локализованного файла соглашения.|


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


