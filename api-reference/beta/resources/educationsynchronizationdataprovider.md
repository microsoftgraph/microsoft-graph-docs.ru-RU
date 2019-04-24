---
title: Тип ресурса Едукатионсинчронизатиондатапровидер
description: 'Представляет исходную схему SIS. Это позволяет системе узнать, как сопоставить входящие данные с схемой Azure Active Directory (Azure AD). '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507046"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="226be-104">Тип ресурса Едукатионсинчронизатиондатапровидер</span><span class="sxs-lookup"><span data-stu-id="226be-104">educationSynchronizationDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="226be-105">Представляет исходную схему SIS.</span><span class="sxs-lookup"><span data-stu-id="226be-105">Represents the source SIS schema.</span></span> <span data-ttu-id="226be-106">Это позволяет системе узнать, как сопоставить входящие данные с схемой Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="226be-106">This allows the system to know how to map the incoming data to the Azure Active Directory (Azure AD) schema.</span></span>

> <span data-ttu-id="226be-107">**Примечание:** Этот сложный тип является абстрактным.</span><span class="sxs-lookup"><span data-stu-id="226be-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="226be-108">Ознакомьтесь со списками определенных типов поставщиков данных.</span><span class="sxs-lookup"><span data-stu-id="226be-108">Refer to the specific types of data providers listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="226be-109">ПроизВодные типы</span><span class="sxs-lookup"><span data-stu-id="226be-109">Derived types</span></span>
| <span data-ttu-id="226be-110">Тип</span><span class="sxs-lookup"><span data-stu-id="226be-110">Type</span></span> | <span data-ttu-id="226be-111">Описание</span><span class="sxs-lookup"><span data-stu-id="226be-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="226be-112">едукатионксвдатапровидер</span><span class="sxs-lookup"><span data-stu-id="226be-112">educationcsvdataprovider</span></span>](educationcsvdataprovider.md) | <span data-ttu-id="226be-113">Используется с CSV-файлами в качестве источника входных данных.</span><span class="sxs-lookup"><span data-stu-id="226be-113">Used with CSV files as the input source.</span></span> |
| [<span data-ttu-id="226be-114">едукатионповерсчулдатапровидер</span><span class="sxs-lookup"><span data-stu-id="226be-114">educationpowerschooldataprovider</span></span>](educationpowerschooldataprovider.md) | <span data-ttu-id="226be-115">Используется с PowerSchool в качестве источника входных данных.</span><span class="sxs-lookup"><span data-stu-id="226be-115">Used with PowerSchool as the input source.</span></span> |
| [<span data-ttu-id="226be-116">едукатиононеростерапидатапровидер</span><span class="sxs-lookup"><span data-stu-id="226be-116">educationonerosterapidataprovider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="226be-117">Используется с API OneRoster в качестве источника входных данных.</span><span class="sxs-lookup"><span data-stu-id="226be-117">Used with OneRoster API as the input source.</span></span> |

## <a name="properties"></a><span data-ttu-id="226be-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="226be-118">Properties</span></span>

<span data-ttu-id="226be-119">Этот тип не представляет свойства.</span><span class="sxs-lookup"><span data-stu-id="226be-119">No properties are exposed by this type.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
