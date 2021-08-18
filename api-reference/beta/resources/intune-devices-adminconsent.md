---
title: тип ресурса adminConsent
description: Сведения о согласии администратора.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d56646299766427a4598ab1073064bfa8ea86a3c405df17b59bb52866b47e75a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227367"
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




