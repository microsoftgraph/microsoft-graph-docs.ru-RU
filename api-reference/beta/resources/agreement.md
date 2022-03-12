---
title: тип ресурса соглашения
description: Представляет настраиваемые условия соглашения об использовании клиента, которое создается и управляется с Azure Active Directory (Azure AD).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: dc91a115d79e47cddbeb7211e2b15aaa7bce9528
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451149"
---
# <a name="agreement-resource-type"></a>тип ресурса соглашения

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет настраиваемые условия соглашения об использовании клиента, которое создается и управляется с Azure Active Directory (Azure AD). Вы можете использовать следующие методы для создания и управления функцией [Azure Active Directory терминов использования](/azure/active-directory/conditional-access/terms-of-use) в соответствии с вашим сценарием.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/termsofusecontainer-post-agreements.md) | [соглашение](agreement.md) | Создайте новое соглашение, разместив в коллекции соглашений. |
| [Перечисление](../api/termsofusecontainer-list-agreements.md) | [коллекция соглашений](agreement.md) | Получите коллекцию объектов соглашения. |
| [Получение](../api/agreement-get.md) | [соглашение](agreement.md) | Чтение свойств и связей объекта соглашения. |
| [Обновление](../api/agreement-update.md) | Нет | Обновление объекта соглашения. |
| [удаление](../api/agreement-delete.md); | Нет | Удаление объекта соглашения. |
|[Приемки списков](../api/agreement-list-acceptances.md)|Коллекция [agreementAcceptance](../resources/agreementacceptance.md)|Сведения о записях приемки для определенного соглашения.|
|[Перечисление agreementAcceptances](../api/user-list-agreementacceptances.md)|Коллекция [agreementAcceptance](../resources/agreementacceptance.md)|Получите приемки соглашения для подписанного пользователя.|
|[Get agreementFile](../api/agreementfile-get.md)|[коллекция agreementFile](../resources/agreementfile.md)|Извлечение сведений из файла по умолчанию для соглашения, включая сведения о языке и версии.|
|[Файлы списка](../api/agreement-list-files.md)|[коллекция agreementFileLocalization](../resources/agreementfilelocalization.md)|Извлечение всех локализованных файлов, связанных с соглашением.|
|[Создание agreementFileLocalization](../api/agreement-post-files.md)|[agreementFileLocalization](../resources/agreementfilelocalization.md)|Создание нового локализованного файла соглашения.|


## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String|Отображение имени соглашения. Имя отображения используется для внутреннего отслеживания соглашения, но не отображается конечным пользователям, которые просматривают соглашение. Поддерживает `$filter` (`eq`).|
|id|String| Только для чтения. Поддерживает `$filter` (`eq`).|
|isPerDeviceAcceptanceRequired|Boolean|Этот параметр позволяет требовать от конечных пользователей принять это соглашение на каждом устройстве, с которое они имеют к нему доступ. Конечный пользователь должен будет зарегистрировать свое устройство в Azure AD, если он этого еще не сделал. Поддерживает `$filter` (`eq`).|
|isViewingBeforeAcceptanceRequired|Boolean|Указывает, должен ли пользователь расширить соглашение перед принятием. Поддерживает `$filter` (`eq`).|
|termsExpiration|[termsExpiration](termsexpiration.md)| Срок действия и периодичность соглашения для всех пользователей.  Поддерживает `$filter` (`eq`).|
|userReacceptRequiredFrequency|Длительность|Продолжительность, после которой пользователь должен повторно принять условия использования. Значение представлено в формате ISO 8601 для длительности.|


## <a name="relationships"></a>Отношения
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|приемки|Коллекция [agreementAcceptance](agreementacceptance.md)|Только для чтения. Сведения о принятии этого соглашения.|
|file|[agreementFile](agreementfile.md) | PDF по умолчанию, связанный с этим соглашением.|
|files|[коллекция agreementFileLocalization](agreementfilelocalization.md)| PDF, связанные с этим соглашением. **Примечание:** Это свойство находится в процессе сноса. Вместо этого  **используйте свойство** file.|


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
