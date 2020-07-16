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
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="50a04-104">Тип ресурса Едукатионсинчронизатиондатапровидер</span><span class="sxs-lookup"><span data-stu-id="50a04-104">educationSynchronizationDataProvider resource type</span></span>

<span data-ttu-id="50a04-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50a04-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50a04-106">Представляет поставщика данных, который будет использоваться в качестве источника синхронизации для объекта [едукатионсинчронизатионпрофиле].</span><span class="sxs-lookup"><span data-stu-id="50a04-106">Represents the data provider to use as the synchronization source for a [educationSynchronizationProfile].</span></span>

> <span data-ttu-id="50a04-107">**Примечание:** Этот сложный тип является абстрактным.</span><span class="sxs-lookup"><span data-stu-id="50a04-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="50a04-108">Ознакомьтесь со списками определенных типов поставщиков данных.</span><span class="sxs-lookup"><span data-stu-id="50a04-108">Refer to the specific types of data providers listed.</span></span>

## <a name="providers"></a><span data-ttu-id="50a04-109">Поставщики</span><span class="sxs-lookup"><span data-stu-id="50a04-109">Providers</span></span>

| <span data-ttu-id="50a04-110">Поставщик данных</span><span class="sxs-lookup"><span data-stu-id="50a04-110">Data Provider</span></span>                                                             | <span data-ttu-id="50a04-111">Description</span><span class="sxs-lookup"><span data-stu-id="50a04-111">Description</span></span>                                                                                        |
|:--------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="50a04-112">[едукатионксвдатапровидер]</span><span class="sxs-lookup"><span data-stu-id="50a04-112">[educationCsvDataProvider]</span></span>                                                | <span data-ttu-id="50a04-113">CSV-файлы, отправленные на [URL-адрес профиля SAS](../api/educationsynchronizationprofile-uploadurl.md)</span><span class="sxs-lookup"><span data-stu-id="50a04-113">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="50a04-114">едукатиононеростерапидатапровидер</span><span class="sxs-lookup"><span data-stu-id="50a04-114">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="50a04-115">API OneRoster 1.1</span><span class="sxs-lookup"><span data-stu-id="50a04-115">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="50a04-116">[едукатионповерсчулдатапровидер]</span><span class="sxs-lookup"><span data-stu-id="50a04-116">[educationPowerSchoolDataProvider]</span></span>                                        | <span data-ttu-id="50a04-117">API PowerSchool</span><span class="sxs-lookup"><span data-stu-id="50a04-117">PowerSchool API</span></span>                                                                                    |

## <a name="properties"></a><span data-ttu-id="50a04-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="50a04-118">Properties</span></span>

<span data-ttu-id="50a04-119">Этот тип не представляет свойства.</span><span class="sxs-lookup"><span data-stu-id="50a04-119">No properties are exposed by this type.</span></span>

[едукатионсинчронизатионпрофиле]: educationsynchronizationprofile.md
[educationsynchronizationprofile]: educationsynchronizationprofile.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[едукатионповерсчулдатапровидер]: educationPowerSchoolDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
