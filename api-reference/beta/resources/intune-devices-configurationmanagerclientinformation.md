---
title: тип ресурса configurationManagerClientInformation
description: Сведения о клиентах Configuration Manager, синхронизированные из SCCM
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0fde63ebef1ce0e8e5ef48252e9014704c768ed8
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58818079"
---
# <a name="configurationmanagerclientinformation-resource-type"></a>тип ресурса configurationManagerClientInformation

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о клиентах Configuration Manager, синхронизированные из SCCM

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|clientIdentifier|String|Id клиента диспетчера конфигурации из SCCM|
|isBlocked|Логический|Клиент диспетчера конфигурации, заблокированный в SCCM|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
  "clientIdentifier": "String",
  "isBlocked": true
}
```



