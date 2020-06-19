---
title: Тип ресурса Едукатионсинчронизатиондатапровидер
description: 'Представляет исходную схему SIS. Это позволяет системе узнать, как сопоставить входящие данные с схемой Azure Active Directory (Azure AD). '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f0691a7157fb189e75e862448069ff8ebdeee9f7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790924"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>Тип ресурса Едукатионсинчронизатиондатапровидер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поставщика данных, который будет использоваться в качестве источника синхронизации для объекта [едукатионсинчронизатионпрофиле].

> **Примечание:** Этот сложный тип является абстрактным. Ознакомьтесь со списками определенных типов поставщиков данных.

## <a name="providers"></a>Поставщики

| Поставщик данных                       | Описание                                                                                        |
| :---------------------------------- | :------------------------------------------------------------------------------------------------- |
| [едукатионксвдатапровидер]          | CSV-файлы, отправленные на [URL-адрес профиля SAS](../api/educationsynchronizationprofile-uploadurl.md) |
| [едукатиононеростерапидатапровидер](educationonerosterapidataprovider.md) | API OneRoster 1.1                                                                                 |
| [едукатионповерсчулдатапровидер]  | API PowerSchool                                                                                    |

## <a name="properties"></a>Свойства

Этот тип не представляет свойства.

[едукатионсинчронизатионпрофиле]: educationsynchronizationprofile.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[едукатионповерсчулдатапровидер]: educationPowerSchoolDataProvider.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
