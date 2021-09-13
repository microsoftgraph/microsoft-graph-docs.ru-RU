---
title: тип ресурса windowsKioskAzureADGroup
description: Класс, используемый для определения группы AzureAD для конфигурации киоска
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c888ad3d14c522813d4959040b1c67b0dbb53777
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086659"
---
# <a name="windowskioskazureadgroup-resource-type"></a>тип ресурса windowsKioskAzureADGroup

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, используемый для определения группы AzureAD для конфигурации киоска


Наследуется [от windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображает имя группы AzureAD, которая будет заблокирована в этой конфигурации киоска|
|groupId|String|ID группы AzureAD, которая будет заблокирована в этой конфигурации киоска|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```



