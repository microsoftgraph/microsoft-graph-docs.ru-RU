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
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="0a940-104">Тип ресурса Едукатионсинчронизатиондатапровидер</span><span class="sxs-lookup"><span data-stu-id="0a940-104">educationSynchronizationDataProvider resource type</span></span>

<span data-ttu-id="0a940-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a940-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a940-106">Представляет поставщика данных, который будет использоваться в качестве источника синхронизации для объекта [едукатионсинчронизатионпрофиле].</span><span class="sxs-lookup"><span data-stu-id="0a940-106">Represents the data provider to use as the synchronization source for a [educationSynchronizationProfile].</span></span>

> [!NOTE]
> <span data-ttu-id="0a940-107">Этот сложный тип является абстрактным.</span><span class="sxs-lookup"><span data-stu-id="0a940-107">This complex type is abstract.</span></span> <span data-ttu-id="0a940-108">Ознакомьтесь со списками определенных типов поставщиков данных.</span><span class="sxs-lookup"><span data-stu-id="0a940-108">Refer to the specific types of data providers listed.</span></span>

## <a name="providers"></a><span data-ttu-id="0a940-109">Поставщики</span><span class="sxs-lookup"><span data-stu-id="0a940-109">Providers</span></span>

| <span data-ttu-id="0a940-110">Поставщик данных</span><span class="sxs-lookup"><span data-stu-id="0a940-110">Data Provider</span></span>                                                             | <span data-ttu-id="0a940-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a940-111">Description</span></span>                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0a940-112">[едукатионксвдатапровидер]</span><span class="sxs-lookup"><span data-stu-id="0a940-112">[educationCsvDataProvider]</span></span>                                                | <span data-ttu-id="0a940-113">CSV-файлы, отправленные на [URL-адрес профиля SAS](../api/educationsynchronizationprofile-uploadurl.md)</span><span class="sxs-lookup"><span data-stu-id="0a940-113">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="0a940-114">едукатиононеростерапидатапровидер</span><span class="sxs-lookup"><span data-stu-id="0a940-114">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="0a940-115">API OneRoster 1.1</span><span class="sxs-lookup"><span data-stu-id="0a940-115">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="0a940-116">[едукатионповерсчулдатапровидер]</span><span class="sxs-lookup"><span data-stu-id="0a940-116">[educationPowerSchoolDataProvider]</span></span>                                        | <span data-ttu-id="0a940-117">API PowerSchool</span><span class="sxs-lookup"><span data-stu-id="0a940-117">PowerSchool API</span></span>                                                                                    |

[едукатионсинчронизатионпрофиле]: educationsynchronizationprofile.md
[educationsynchronizationprofile]: educationsynchronizationprofile.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[едукатионповерсчулдатапровидер]: educationPowerSchoolDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
