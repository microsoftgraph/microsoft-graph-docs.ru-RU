---
title: Тип ресурса Кустомсубжекталтернативенаме
description: Определение альтернативного имени настраиваемой темы
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a2e54e6d3c0ddea77758b083e5d2f979dc7f49b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526938"
---
# <a name="customsubjectalternativename-resource-type"></a>Тип ресурса Кустомсубжекталтернативенаме

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение альтернативного имени настраиваемой темы

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|сантипе|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|Настраиваемый тип SAN. Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|name|String|Настраиваемое имя сети хранения данных|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```



