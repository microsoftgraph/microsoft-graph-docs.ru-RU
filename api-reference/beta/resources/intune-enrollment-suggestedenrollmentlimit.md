---
title: Тип ресурса Сугжестеденроллментлимит
description: Ресурс Сугжестеденроллментлимит представляет Рекомендуемое предельное значение регистрации при наличии типа регистрации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 880fb5d77c7fa16a23349918973a33ba0952e07a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256262"
---
# <a name="suggestedenrollmentlimit-resource-type"></a><span data-ttu-id="cc68c-103">Тип ресурса Сугжестеденроллментлимит</span><span class="sxs-lookup"><span data-stu-id="cc68c-103">suggestedEnrollmentLimit resource type</span></span>

<span data-ttu-id="cc68c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc68c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc68c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc68c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc68c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc68c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc68c-107">Ресурс Сугжестеденроллментлимит представляет Рекомендуемое предельное значение регистрации при наличии типа регистрации.</span><span class="sxs-lookup"><span data-stu-id="cc68c-107">The suggestedEnrollmentLimit resource represents the suggested enrollment limit when given an enrollment type.</span></span>

## <a name="properties"></a><span data-ttu-id="cc68c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc68c-108">Properties</span></span>
|<span data-ttu-id="cc68c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc68c-109">Property</span></span>|<span data-ttu-id="cc68c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cc68c-110">Type</span></span>|<span data-ttu-id="cc68c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cc68c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc68c-112">сугжестеддаилилимит</span><span class="sxs-lookup"><span data-stu-id="cc68c-112">suggestedDailyLimit</span></span>|<span data-ttu-id="cc68c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="cc68c-113">Int32</span></span>|<span data-ttu-id="cc68c-114">Предполагаемое количество заявок в течение дня</span><span class="sxs-lookup"><span data-stu-id="cc68c-114">The suggested enrollment limit within a day</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc68c-115">Связи</span><span class="sxs-lookup"><span data-stu-id="cc68c-115">Relationships</span></span>
<span data-ttu-id="cc68c-116">Нет</span><span class="sxs-lookup"><span data-stu-id="cc68c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc68c-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc68c-117">JSON Representation</span></span>
<span data-ttu-id="cc68c-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc68c-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.suggestedEnrollmentLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.suggestedEnrollmentLimit",
  "suggestedDailyLimit": 1024
}
```




