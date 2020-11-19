---
title: Тип ресурса Секуритибаселинеконтрибутингполици
description: Состояние соответствия базовой безопасности параметру для устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f62299f39d4e3670fc586a4dc07d352a992398e0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209348"
---
# <a name="securitybaselinecontributingpolicy-resource-type"></a>Тип ресурса Секуритибаселинеконтрибутингполици

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние соответствия базовой безопасности параметру для устройства

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Идентификатор|String|Уникальный идентификатор политики|
|displayName|String|Имя политики|
|sourceType|[секуритибаселинеполицисаурцетипе](../resources/intune-deviceintent-securitybaselinepolicysourcetype.md)|Источник создания политики. Возможные значения: `deviceConfiguration`, `deviceIntent`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.securityBaselineContributingPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineContributingPolicy",
  "sourceId": "String",
  "displayName": "String",
  "sourceType": "String"
}
```




