---
title: тип ресурса соглашения
description: Представляет настраиваемые условия соглашения об использовании клиента, которое создается и управляется с Azure Active Directory (Azure AD).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 6fe44635130eabe20826c85861ccaccb894658c0
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651437"
---
# <a name="agreement-resource-type"></a>тип ресурса соглашения

Пространство имен: microsoft.graph

Представляет настраиваемые условия соглашения об использовании клиента, которое создается и управляется с Azure Active Directory (Azure AD). Вы можете использовать следующие методы для создания и управления функцией [Azure Active Directory терминов использования](/azure/active-directory/conditional-access/terms-of-use) в соответствии с вашим сценарием.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список соглашений](../api/termsofusecontainer-list-agreements.md) | [коллекция соглашений](agreement.md) | Получите коллекцию объектов соглашения. |
| [Создание соглашений](../api/termsofusecontainer-post-agreements.md) | [соглашение](agreement.md) | Создайте новое соглашение, разместив в коллекции соглашений. |
| [Получение соглашения](../api/agreement-get.md) | [соглашение](agreement.md) | Чтение свойств и связей объекта соглашения. |
| [Обновление соглашения](../api/agreement-update.md) | [соглашение](agreement.md) | Обновление объекта соглашения. |
| [Удаление соглашения](../api/agreement-delete.md) | Нет | Удаление объекта соглашения. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|Строка|Отображение имени соглашения. Имя отображения используется для внутреннего отслеживания соглашения, но не отображается конечным пользователям, которые просматривают соглашение.|
|id|String| Идентификатор соглашения. Только для чтения.|
|isPerDeviceAcceptanceRequired|Boolean|Указывает, должны ли конечные пользователи принимать это соглашение на каждом устройстве, с которое они имеют к нему доступ. Конечный пользователь должен зарегистрировать свое устройство в Azure AD, если он еще этого не сделал.|
|isViewingBeforeAcceptanceRequired|Boolean|Указывает, должен ли пользователь расширить соглашение перед принятием.|
|termsExpiration|[termsExpiration](termsexpiration.md)| Срок действия и периодичность соглашения для всех пользователей. |
|userReacceptRequiredFrequency|Длительность|Продолжительность, после которой пользователь должен повторно принять условия использования. Значение представлено в формате ISO 8601 для длительности.|


## <a name="relationships"></a>Отношения
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|приемки|Коллекция [agreementAcceptance](agreementacceptance.md)|Только для чтения. Сведения о принятии этого соглашения.|
|file|[agreementFile](agreementfile.md) | PDF по умолчанию, связанный с этим соглашением.|
|files|[коллекция agreementFileLocalization](agreementfilelocalization.md)| PDF, связанные с этим соглашением. Это свойство находится в процессе сноса. Вместо этого  **используйте свойство** file.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.agreement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.agreement",
  "id": "String (identifier)",
  "displayName": "String",
  "termsExpiration": {
    "@odata.type": "microsoft.graph.termsExpiration"
  },
  "userReacceptRequiredFrequency": "String (duration)",
  "isViewingBeforeAcceptanceRequired": "Boolean",
  "isPerDeviceAcceptanceRequired": "Boolean"
}
```
