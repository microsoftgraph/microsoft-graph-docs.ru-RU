---
title: Тип ресурса educationSynchronizationDataProvider
description: 'Представляет схему SIS источника. Это позволяет системы, чтобы знать, как сопоставление входящих данных схемы Azure Active Directory (Azure AD). '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515498"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="a0ceb-104">Тип ресурса educationSynchronizationDataProvider</span><span class="sxs-lookup"><span data-stu-id="a0ceb-104">educationSynchronizationDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0ceb-105">Представляет схему SIS источника.</span><span class="sxs-lookup"><span data-stu-id="a0ceb-105">Represents the source SIS schema.</span></span> <span data-ttu-id="a0ceb-106">Это позволяет системы, чтобы знать, как сопоставление входящих данных схемы Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a0ceb-106">This allows the system to know how to map the incoming data to the Azure Active Directory (Azure AD) schema.</span></span>

> <span data-ttu-id="a0ceb-107">**Примечание:** В данном сложном типе абстрактный.</span><span class="sxs-lookup"><span data-stu-id="a0ceb-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="a0ceb-108">Обращайтесь к определенным типам поставщиков данных из списка.</span><span class="sxs-lookup"><span data-stu-id="a0ceb-108">Refer to the specific types of data providers listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="a0ceb-109">Производные типы</span><span class="sxs-lookup"><span data-stu-id="a0ceb-109">Derived types</span></span>
| <span data-ttu-id="a0ceb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a0ceb-110">Type</span></span> | <span data-ttu-id="a0ceb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a0ceb-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="a0ceb-112">educationcsvdataprovider</span><span class="sxs-lookup"><span data-stu-id="a0ceb-112">educationcsvdataprovider</span></span>](educationcsvdataprovider.md) | <span data-ttu-id="a0ceb-113">Использовать с помощью CSV-файлов в качестве источника ввода.</span><span class="sxs-lookup"><span data-stu-id="a0ceb-113">Used with CSV files as the input source.</span></span> |
| [<span data-ttu-id="a0ceb-114">educationpowerschooldataprovider</span><span class="sxs-lookup"><span data-stu-id="a0ceb-114">educationpowerschooldataprovider</span></span>](educationpowerschooldataprovider.md) | <span data-ttu-id="a0ceb-115">Используется с PowerSchool в качестве источника ввода.</span><span class="sxs-lookup"><span data-stu-id="a0ceb-115">Used with PowerSchool as the input source.</span></span> |
| [<span data-ttu-id="a0ceb-116">educationonerosterapidataprovider</span><span class="sxs-lookup"><span data-stu-id="a0ceb-116">educationonerosterapidataprovider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="a0ceb-117">Использовать с использованием интерфейса API OneRoster в качестве источника ввода.</span><span class="sxs-lookup"><span data-stu-id="a0ceb-117">Used with OneRoster API as the input source.</span></span> |

## <a name="properties"></a><span data-ttu-id="a0ceb-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0ceb-118">Properties</span></span>

<span data-ttu-id="a0ceb-119">С этого типа свойств не представлено.</span><span class="sxs-lookup"><span data-stu-id="a0ceb-119">No properties are exposed by this type.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
