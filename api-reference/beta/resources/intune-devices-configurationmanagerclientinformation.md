---
title: тип ресурса configurationManagerClientInformation
description: Сведения о клиентах Configuration Manager, синхронизированные из SCCM
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3af9373c8359ed28465cb580057d06850dcb3504
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026940"
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
|isBlocked|Boolean|Клиент диспетчера конфигурации, заблокированный в SCCM|

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



