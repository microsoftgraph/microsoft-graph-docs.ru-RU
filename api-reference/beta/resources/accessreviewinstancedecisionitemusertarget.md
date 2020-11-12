---
title: Тип ресурса АкцессревиевинстанцедеЦисионитемусертаржет
description: Представляет целевой объект проверки от имени пользователя.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aa2117895599ba1d2c4b9829b7cad22b581f2055
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001063"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a><span data-ttu-id="e6107-103">Тип ресурса АкцессревиевинстанцедеЦисионитемусертаржет</span><span class="sxs-lookup"><span data-stu-id="e6107-103">accessReviewInstanceDecisionItemUserTarget resource type</span></span>

<span data-ttu-id="e6107-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6107-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6107-105">Представляет удостоверение пользователя в ходе рецензирования в [акцессревиевинстанце](accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="e6107-105">Represents a user identity under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="e6107-106">Наследуется от [акцессревиевинстанцедеЦисионитемтаржет](../resources/accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="e6107-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e6107-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6107-107">Properties</span></span>
|<span data-ttu-id="e6107-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6107-108">Property</span></span>|<span data-ttu-id="e6107-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e6107-109">Type</span></span>|<span data-ttu-id="e6107-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e6107-110">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="e6107-111">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e6107-111">userDisplayName</span></span> | <span data-ttu-id="e6107-112">String</span><span class="sxs-lookup"><span data-stu-id="e6107-112">String</span></span> | <span data-ttu-id="e6107-113">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="e6107-113">The name of user.</span></span> |
| <span data-ttu-id="e6107-114">userId</span><span class="sxs-lookup"><span data-stu-id="e6107-114">userId</span></span> | <span data-ttu-id="e6107-115">String</span><span class="sxs-lookup"><span data-stu-id="e6107-115">String</span></span> | <span data-ttu-id="e6107-116">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="e6107-116">The identifier of user.</span></span> |
| <span data-ttu-id="e6107-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e6107-117">userPrincipalName</span></span> | <span data-ttu-id="e6107-118">String</span><span class="sxs-lookup"><span data-stu-id="e6107-118">String</span></span> | <span data-ttu-id="e6107-119">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="e6107-119">The user principal name.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e6107-120">Связи</span><span class="sxs-lookup"><span data-stu-id="e6107-120">Relationships</span></span>
<span data-ttu-id="e6107-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e6107-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6107-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e6107-122">JSON representation</span></span>
<span data-ttu-id="e6107-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6107-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemUserTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
