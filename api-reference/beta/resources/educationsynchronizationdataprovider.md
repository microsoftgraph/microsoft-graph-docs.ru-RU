---
title: Тип ресурса Едукатионсинчронизатиондатапровидер
description: 'Представляет исходную схему SIS. Это позволяет системе узнать, как сопоставить входящие данные с схемой Azure Active Directory (Azure AD). '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 952d0a7f9a40f41ad87d632386d9d567036cfec7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989656"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>Тип ресурса Едукатионсинчронизатиондатапровидер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поставщика данных, который будет использоваться в качестве источника синхронизации для объекта [едукатионсинчронизатионпрофиле].

> [!NOTE]
> Этот сложный тип является абстрактным. Ознакомьтесь со списками определенных типов поставщиков данных.

## <a name="providers"></a>Поставщики

| Поставщик данных                                                             | Описание                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| [едукатионксвдатапровидер]                                                | CSV-файлы, отправленные на [URL-адрес профиля SAS](../api/educationsynchronizationprofile-uploadurl.md) |
| [едукатиононеростерапидатапровидер](educationonerosterapidataprovider.md) | API OneRoster 1.1                                                                                 |
| [едукатионповерсчулдатапровидер]                                        | API PowerSchool                                                                                    |

[едукатионсинчронизатионпрофиле]: educationsynchronizationprofile.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[едукатионповерсчулдатапровидер]: educationPowerSchoolDataProvider.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md


