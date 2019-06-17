---
title: Тип ресурса Adminconsent.
description: Сведения о согласия администратора.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a25dd46c8f1f8efdc3149472dae88910774e44a9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983374"
---
# <a name="adminconsent-resource-type"></a>Тип ресурса Adminconsent.

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о согласия администратора.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Шареапнсдата|[Админконсентстате](../resources/intune-devices-adminconsentstate.md)|Разрешение администратора о предоставлении общего доступа к данным о пользователях и устройствах в Apple. Возможные значения: `notConfigured`, `granted`, `notGranted`.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```





