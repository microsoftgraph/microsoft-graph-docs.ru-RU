---
title: тип ресурса cloudPcDomainJoinConfiguration
description: Представляет собой заданная конфигурация того, как предварительное устройство облачного ПК будет присоединяться к Azure Active Directory.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 3f35fb4a2aca6e7d0abd197e0c982038de3729ca
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587639"
---
# <a name="cloudpcdomainjoinconfiguration-resource-type"></a>тип ресурса cloudPcDomainJoinConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет собой заданная конфигурация того, как к Azure Active Directory Azure AD будет присоединяться предварительное устройство облачного ПК.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|onPremisesConnectionId|String|ID сетевого подключения Azure, который соответствует ИТ-администраторам виртуальной сети, должен использовать политику продюсинга при создании облачных компьютеров. Это свойство можно использовать в обоих типах присоединяться к доменам: _к Azure AD_ присоединились или _к Гибридной Azure AD_. Если вы введите **onPremisesConnectionId**, оставьте **имя regionName** пустым.|
|regionName|Строка|Поддерживаемый регион Azure, в котором ИТ-администратору нужна политика обеспечения создания облачных компьютеров. Виртуальная сеть будет создана и управляется Windows 365 службой. Это можно ввести только в том случае, если ИТ-администратор выбирает, что Azure AD присоединяется к типу присоединяемого домена. Если введите **имя regionName**, оставьте **наPremisesConnectionId** пустым.|
|type|[cloudPcDomainJoinType](#cloudpcdomainjointype-values)|Указывает, как к Azure AD будет присоединяться к предварительному облачному компьютеру. Если вы выберете `hybridAzureADJoin` тип, уставьте только значение свойства **onPremisesConnectionId** и оставьте **имя regionName** пустым. Если вы выбираете `azureADJoin` тип, уведите значение для **onPremisesConnectionId или** **regionName**. Допустимые значения: `azureADJoin`, `hybridAzureADJoin`, `unknownFutureValue`.|

### <a name="cloudpcdomainjointype-values"></a>значения cloudPcDomainJoinType

|Member|Описание|
|:---|:---|
|azureADJoin|Присоединилась только к Azure AD. Пользователи только для облачных и гибридных сетей могут быть назначены и войти в облачный компьютер.|
|hybridAzureADJoin|Присоединились к локальной AD и Azure AD. Только гибридные пользователи могут быть назначены и войти в облачный компьютер.|
|unknownFutureValue|Эволюционирующее значение sentinel. Не следует использовать.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcDomainJoinConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDomainJoinConfiguration",
  "type": "String",
  "regionName": "String",
  "onPremisesConnectionId": "String"
}
```
