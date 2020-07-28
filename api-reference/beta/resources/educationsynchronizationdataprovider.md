---
title: Тип ресурса Едукатионсинчронизатиондатапровидер
description: 'Представляет исходную схему SIS. Это позволяет системе узнать, как сопоставить входящие данные с схемой Azure Active Directory (Azure AD). '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f20bea087a23f14acd7184c5211d21687409897a
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434972"
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
