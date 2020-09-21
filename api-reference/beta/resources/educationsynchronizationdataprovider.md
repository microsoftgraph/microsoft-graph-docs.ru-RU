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
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="97591-104">Тип ресурса Едукатионсинчронизатиондатапровидер</span><span class="sxs-lookup"><span data-stu-id="97591-104">educationSynchronizationDataProvider resource type</span></span>

<span data-ttu-id="97591-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97591-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97591-106">Представляет поставщика данных, который будет использоваться в качестве источника синхронизации для объекта [едукатионсинчронизатионпрофиле].</span><span class="sxs-lookup"><span data-stu-id="97591-106">Represents the data provider to use as the synchronization source for a [educationSynchronizationProfile].</span></span>

> [!NOTE]
> <span data-ttu-id="97591-107">Этот сложный тип является абстрактным.</span><span class="sxs-lookup"><span data-stu-id="97591-107">This complex type is abstract.</span></span> <span data-ttu-id="97591-108">Ознакомьтесь со списками определенных типов поставщиков данных.</span><span class="sxs-lookup"><span data-stu-id="97591-108">Refer to the specific types of data providers listed.</span></span>

## <a name="providers"></a><span data-ttu-id="97591-109">Поставщики</span><span class="sxs-lookup"><span data-stu-id="97591-109">Providers</span></span>

| <span data-ttu-id="97591-110">Поставщик данных</span><span class="sxs-lookup"><span data-stu-id="97591-110">Data Provider</span></span>                                                             | <span data-ttu-id="97591-111">Описание</span><span class="sxs-lookup"><span data-stu-id="97591-111">Description</span></span>                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="97591-112">[едукатионксвдатапровидер]</span><span class="sxs-lookup"><span data-stu-id="97591-112">[educationCsvDataProvider]</span></span>                                                | <span data-ttu-id="97591-113">CSV-файлы, отправленные на [URL-адрес профиля SAS](../api/educationsynchronizationprofile-uploadurl.md)</span><span class="sxs-lookup"><span data-stu-id="97591-113">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="97591-114">едукатиононеростерапидатапровидер</span><span class="sxs-lookup"><span data-stu-id="97591-114">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="97591-115">API OneRoster 1.1</span><span class="sxs-lookup"><span data-stu-id="97591-115">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="97591-116">[едукатионповерсчулдатапровидер]</span><span class="sxs-lookup"><span data-stu-id="97591-116">[educationPowerSchoolDataProvider]</span></span>                                        | <span data-ttu-id="97591-117">API PowerSchool</span><span class="sxs-lookup"><span data-stu-id="97591-117">PowerSchool API</span></span>                                                                                    |

[едукатионсинчронизатионпрофиле]: educationsynchronizationprofile.md
[educationsynchronizationprofile]: educationsynchronizationprofile.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[едукатионповерсчулдатапровидер]: educationPowerSchoolDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md


