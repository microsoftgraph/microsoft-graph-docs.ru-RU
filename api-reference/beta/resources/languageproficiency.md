---
title: Тип ресурса ЛангуажепрофиЦиенци
description: Тип ресурса ЛангуажепрофиЦиенци
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a024cd339194f79133201a91dd93213f1db9042e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812823"
---
# <a name="languageproficiency-resource-type"></a>Тип ресурса ЛангуажепрофиЦиенци

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о языках, добавленных пользователем в свой [профиль](profile.md).

Наследуется от [итемфацет](itemFacet.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список языков](../api/profile-list-languages.md)|Коллекция [лангуажепрофиЦиенци](../resources/languageproficiency.md)|Получение ресурсов ЛангуажепрофиЦиенци из свойства навигации для языков.|
|[Создание ЛангуажепрофиЦиенци](../api/profile-post-languages.md)|[лангуажепрофиЦиенци](../resources/languageproficiency.md)|Создание нового объекта ЛангуажепрофиЦиенци.|
|[Получение ЛангуажепрофиЦиенци](../api/languageproficiency-get.md)|[лангуажепрофиЦиенци](../resources/languageproficiency.md)|Чтение свойств и связей объекта [лангуажепрофиЦиенци](../resources/languageproficiency.md) .|
|[Обновление ЛангуажепрофиЦиенци](../api/languageproficiency-update.md)|[лангуажепрофиЦиенци](../resources/languageproficiency.md)|Обновление свойств объекта [лангуажепрофиЦиенци](../resources/languageproficiency.md) .|
|[Удаление ЛангуажепрофиЦиенци](../api/languageproficiency-delete.md)|Нет|Удаляет объект [лангуажепрофиЦиенци](../resources/languageproficiency.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|displayName|String|Содержит имя языка в длинном формате. |
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|ознакомлен|лангуажепрофиЦиенцилевел|Представляет сведения о том, как пользователи читают сведения о языке, представленном объектом. Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|произносимого|лангуажепрофиЦиенцилевел|Представляет знание пользователей для языка, представленного объектом. Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.|
|tag|String|Содержит четырехзначный BCP47 Name для языка (EN-US, No-NetBIOS, en-AU).|
|образом|лангуажепрофиЦиенцилевел|Представляет пользователей, которым предназначено знание языка, представленного объектом. Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.languageProficiency",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.languageProficiency",
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
  "displayName": "String",
  "tag": "String",
  "spoken": "String",
  "written": "String",
  "reading": "String"
}
```
