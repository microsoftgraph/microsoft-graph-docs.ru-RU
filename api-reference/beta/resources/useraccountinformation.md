---
title: Тип ресурса Усераккаунтинформатион
description: Тип ресурса Усераккаунтинформатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 9bcd0553c51d75724f28737321f463bcab034306
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057915"
---
# <a name="useraccountinformation-resource-type"></a>Тип ресурса Усераккаунтинформатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения, специально связанные с учетной записью пользователя, будь то учетная запись Azure AD или учетная запись Майкрософт. Идентификатор сущности задается соответствующим идентификаторам Azure AD AD или CID учетной записи Майкрософт соответственно. Эти поля доступны только для чтения через Microsoft Graph и должны редактироваться с помощью профиля пользователя или администратора клиента для соответствующего интерфейса.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список учетных записей](../api/profile-list-accounts.md)|Коллекция [усераккаунтинформатион](../resources/useraccountinformation.md)|Получение ресурсов Усераккаунтинформатион из свойства навигации учетной записи.|
|[Создание Усераккаунтинформатион](../api/profile-post-accounts.md)|[усераккаунтинформатион](../resources/useraccountinformation.md)|Создание нового объекта Усераккаунтинформатион.|
|[Получение Усераккаунтинформатион](../api/useraccountinformation-get.md)|[усераккаунтинформатион](../resources/useraccountinformation.md)|Чтение свойств и связей объекта [усераккаунтинформатион](../resources/useraccountinformation.md) .|
|[Обновление Усераккаунтинформатион](../api/useraccountinformation-update.md)|[усераккаунтинформатион](../resources/useraccountinformation.md)|Обновление свойств объекта [усераккаунтинформатион](../resources/useraccountinformation.md) .|
|[Удаление Усераккаунтинформатион](../api/useraccountinformation-delete.md)|Нет|Удаляет объект [усераккаунтинформатион](../resources/useraccountinformation.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|ageGroup|String|Показывает группу возрастных пользователей. Допустимые `null` значения `minor` , `notAdult` и `adult` они создаются каталогом и не могут быть изменены.|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|countryCode|String|Содержит двухбуквенный код страны, связанный с учетной записью пользователя.  |
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|преферредлангуажетаг|[localeInfo](../resources/localeinfo.md)|Содержит язык, который пользователь связал с учетной записью как предпочитаемый.   |
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|userPrincipalName|String|Имя участника-пользователя (UPN) пользователя, связанного с учетной записью.   |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAccountInformation",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {
    "@odata.type": "microsoft.graph.localeInfo"
  },
  "userPrincipalName": "String"
}
```


