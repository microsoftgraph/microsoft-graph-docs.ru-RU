---
title: тип ресурса userExperienceAnalyticsSettings
description: Анализ пользовательских интерфейсов — это рекомендация по улучшению показателей аналитики пользовательских интерфейсов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 877e710d00405f3b9a592cd7eb2501d25495d0a61237ea5acc62f6cb9e4f38d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54185686"
---
# <a name="userexperienceanalyticssettings-resource-type"></a>тип ресурса userExperienceAnalyticsSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Анализ пользовательских интерфейсов — это рекомендация по улучшению показателей аналитики пользовательских интерфейсов.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|configurationManagerDataConnectorConfigured|Логический|True, если присоединение к клиенту настроено. Если настроено, подключенные к клиенту SCCM устройства будут показываться в отчетах UXA.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsSettings",
  "configurationManagerDataConnectorConfigured": true
}
```




