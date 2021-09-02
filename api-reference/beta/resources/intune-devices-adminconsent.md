---
title: тип ресурса adminConsent
description: Сведения о согласии администратора.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dcf849e8c44e68bb4b76417748dbe795e0dd5852
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58816517"
---
# <a name="adminconsent-resource-type"></a>тип ресурса adminConsent

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о согласии администратора.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|shareAPNSData|[adminConsentState](../resources/intune-devices-adminconsentstate.md)|Состояние согласия администратора для обмена данными пользователей и устройств в Apple. Возможные значения: `notConfigured`, `granted`, `notGranted`.|
|shareUserExperienceAnalyticsData|[adminConsentState](../resources/intune-devices-adminconsentstate.md)|Получает или задает согласие администратора на обмен данными аналитики пользовательских интерфейсов. Возможные значения: `notConfigured`, `granted`, `notGranted`.|

## <a name="relationships"></a>Связи
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
  "shareAPNSData": "String",
  "shareUserExperienceAnalyticsData": "String"
}
```



