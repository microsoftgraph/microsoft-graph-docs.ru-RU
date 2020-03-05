---
title: Тип ресурса Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари
description: Содержит свойства сводки по развертыванию дополнительной политики Виндовсдефендераппликатионконтрол.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d1eb05a259921c4be649de50d442eaa3938c2ce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523242"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-resource-type"></a>Тип ресурса Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари

Пространство имен: Microsoft. Graph

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



