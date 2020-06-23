---
title: Тип ресурса Едукатионсинчронизатиондатапровидер
description: 'Представляет исходную схему SIS. Это позволяет системе узнать, как сопоставить входящие данные с схемой Azure Active Directory (Azure AD). '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: be0f50ec3cff0a8eec91cd43b4bb08371db806f3
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846165"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>Тип ресурса Едукатионсинчронизатиондатапровидер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поставщика данных, который будет использоваться в качестве источника синхронизации для объекта [едукатионсинчронизатионпрофиле].

> **Примечание:** Этот сложный тип является абстрактным. Ознакомьтесь со списками определенных типов поставщиков данных.

## <a name="providers"></a>Поставщики

| Поставщик данных                                                             | Description                                                                                        |
|:--------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [едукатионксвдатапровидер]                                                | CSV-файлы, отправленные на [URL-адрес профиля SAS](../api/educationsynchronizationprofile-uploadurl.md) |
| [едукатиононеростерапидатапровидер](educationonerosterapidataprovider.md) | API OneRoster 1.1                                                                                 |
| [едукатионповерсчулдатапровидер]                                        | API PowerSchool                                                                                    |

## <a name="properties"></a>Свойства

Этот тип не представляет свойства.

[едукатионсинчронизатионпрофиле]: educationsynchronizationprofile.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[едукатионповерсчулдатапровидер]: educationPowerSchoolDataProvider.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
