---
title: тип ресурса cloudPcDomainJoinConfiguration
description: Представляет собой заданная конфигурация того, как предварительное устройство облачного ПК будет присоединяться к Azure Active Directory.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7bb82c080ce1987bba8d0e9dafe9ba2fc49e16a1
ms.sourcegitcommit: c00c61ce35a6f204a9907aa6f2644ea7a86a5b6e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2021
ms.locfileid: "60805572"
---
# <a name="cloudpcdomainjoinconfiguration-resource-type"></a>тип ресурса cloudPcDomainJoinConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет собой заданная конфигурация того, как к Azure Active Directory Azure AD будет присоединяться предварительное устройство облачного ПК.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|onPremisesConnectionId|Строка|ИД локального подключения, который соответствует ИТ-администраторам виртуальной сети, необходимо использовать политику обеспечения безопасности при создании облачных компьютеров. Это свойство можно использовать в обоих типах присоединяться к доменам: _к Azure AD_ присоединились или _к Гибридной Azure AD присоединились._ Если вы введите **onPremisesConnectionId,** оставьте **имя regionName** пустым.|
|regionName|Строка|Поддерживаемый регион Azure, в котором ИТ-администратору нужна политика обеспечения создания облачных компьютеров. Виртуальная сеть будет создана и управляется службой Windows 365. Это можно ввести только в том случае, если ИТ-администратор выбирает, что Azure AD присоединяется к типу присоединяемого домена. Если вы введите **имя regionName,** оставьте **наPremisesConnectionId** пустым.|
|type|[cloudPcDomainJoinType](#cloudpcdomainjointype-values)|Указывает, как к Azure AD будет присоединяться к предварительному облачному компьютеру. Если вы выберете тип, уставьте только значение свойства `hybridAzureADJoin` **onPremisesConnectionId** и оставьте **имя regionName** пустым. Если вы выбираете `azureADJoin` тип, уведите значение для **onPremisesConnectionId** или **regionName.** Допустимые значения: `azureADJoin`, `hybridAzureADJoin`, `unknownFutureValue`.|

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
