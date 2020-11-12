---
title: Тип ресурса АкцессревиевинстанцедеЦисионитемсервицепринЦипалтаржет
description: Представляет целевой объект проверки в качестве целевого объекта участника службы.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e9943a287dd28a44f3b36eae1a92d1b2c385496c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001066"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a><span data-ttu-id="42474-103">Тип ресурса АкцессревиевинстанцедеЦисионитемсервицепринЦипалтаржет</span><span class="sxs-lookup"><span data-stu-id="42474-103">accessReviewInstanceDecisionItemServicePrincipalTarget resource type</span></span>

<span data-ttu-id="42474-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42474-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="42474-105">Представляет участника службы в разделе "Обзор" в [акцессревиевинстанце](accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="42474-105">Represents a service principal under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="42474-106">Наследуется от [акцессревиевинстанцедеЦисионитемтаржет](../resources/accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="42474-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="42474-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="42474-107">Properties</span></span>
| <span data-ttu-id="42474-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="42474-108">Property</span></span> | <span data-ttu-id="42474-109">Тип</span><span class="sxs-lookup"><span data-stu-id="42474-109">Type</span></span> | <span data-ttu-id="42474-110">Описание</span><span class="sxs-lookup"><span data-stu-id="42474-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="42474-111">сервицепринЦипалид</span><span class="sxs-lookup"><span data-stu-id="42474-111">servicePrincipalID</span></span> | <span data-ttu-id="42474-112">Строка</span><span class="sxs-lookup"><span data-stu-id="42474-112">String</span></span> | <span data-ttu-id="42474-113">Идентификатор субъекта-службы, доступ к которому просматривается.</span><span class="sxs-lookup"><span data-stu-id="42474-113">The identifier of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="42474-114">сервицепринЦипалдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="42474-114">servicePrincipalDisplayName</span></span> | <span data-ttu-id="42474-115">Строка</span><span class="sxs-lookup"><span data-stu-id="42474-115">String</span></span> | <span data-ttu-id="42474-116">Отображаемое имя субъекта-службы, доступ к которому просматривается.</span><span class="sxs-lookup"><span data-stu-id="42474-116">The display name of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="42474-117">appId</span><span class="sxs-lookup"><span data-stu-id="42474-117">appId</span></span> | <span data-ttu-id="42474-118">String</span><span class="sxs-lookup"><span data-stu-id="42474-118">String</span></span> | <span data-ttu-id="42474-119">AppId для анализируемого объекта участника службы.</span><span class="sxs-lookup"><span data-stu-id="42474-119">The appId for the service principal entity being reviewed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="42474-120">Связи</span><span class="sxs-lookup"><span data-stu-id="42474-120">Relationships</span></span>
<span data-ttu-id="42474-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="42474-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="42474-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="42474-122">JSON representation</span></span>
<span data-ttu-id="42474-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42474-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget",
  "servicePrincipalId": "String",
  "servicePrincipalDisplayName": "String",
  "appId": "String"
}
```
