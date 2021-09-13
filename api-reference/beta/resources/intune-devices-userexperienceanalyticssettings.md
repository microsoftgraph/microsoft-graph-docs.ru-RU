---
title: тип ресурса userExperienceAnalyticsSettings
description: Анализ пользовательских интерфейсов — это рекомендация по улучшению показателей аналитики пользовательских интерфейсов.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67d42f2c7e42fa9ad05a83e59ab5c046b9f08af6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046934"
---
# <a name="userexperienceanalyticssettings-resource-type"></a>тип ресурса userExperienceAnalyticsSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Анализ пользовательских интерфейсов — это рекомендация по улучшению показателей аналитики пользовательских интерфейсов.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|configurationManagerDataConnectorConfigured|Логическое|True, если присоединение к клиенту настроено. Если настроено, подключенные к клиенту SCCM устройства будут показываться в отчетах UXA.|

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



