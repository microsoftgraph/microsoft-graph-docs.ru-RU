---
title: тип ресурса educationSynchronizationDataProvider
description: 'Представляет схему источника SIS. Это позволяет системе составить карту входящих данных с схемой Azure Active Directory Azure AD. '
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 869b24f5db8619caf3d60c17538f7ed4f8d932a5
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225758"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>тип ресурса educationSynchronizationDataProvider

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поставщика данных, который будет использовать в качестве источника синхронизации [для educationSynchronizationProfile.]

> [!NOTE]
> Этот сложный тип абстрактный. Обратитесь к определенным типам перечисленных поставщиков данных.


**Поставщики**

| Поставщик данных                                                             | Описание                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| [educationCsvDataProvider]                                                | CSV-файлы, загруженные на [URL-адрес SAS профиля](../api/educationsynchronizationprofile-uploadurl.md) |
| [educationOneRosterApiDataProvider](educationonerosterapidataprovider.md) | OneRoster v1.1 API                                                                                 |
| [educationPowerSchoolDataProvider]                                        | API PowerSchool                                                                                    |

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationDataProvider"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationDataProvider"
}
```


[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
