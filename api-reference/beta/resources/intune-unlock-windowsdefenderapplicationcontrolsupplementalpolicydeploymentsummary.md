---
title: Тип ресурса Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари
description: Содержит свойства сводки по развертыванию дополнительной политики Виндовсдефендераппликатионконтрол.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c16cdd6518998f6979260462d844cefa072f2061
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449561"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-resource-type"></a>Тип ресурса Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства сводки по развертыванию дополнительной политики Виндовсдефендераппликатионконтрол.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-get.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Чтение свойств и связей объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) .|
|[Обновление Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-update.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Обновление свойств объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|деплойеддевицекаунт|Int32|Количество устройств, успешно развернутых в этой дополнительной политике Виндовсдефендераппликатионконтрол.|
|failedDeviceCount|Int32|Количество устройств, которые не удалось развернуть эту дополнительную политику Виндовсдефендераппликатионконтрол.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary",
  "id": "String (identifier)",
  "deployedDeviceCount": 1024,
  "failedDeviceCount": 1024
}
```



