---
title: Тип ресурса Сугжестеденроллментлимит
description: Ресурс Сугжестеденроллментлимит представляет Рекомендуемое предельное значение регистрации при наличии типа регистрации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99efb75bcf52b841dcf67741045b7207a85eb3cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082116"
---
# <a name="suggestedenrollmentlimit-resource-type"></a><span data-ttu-id="b60da-103">Тип ресурса Сугжестеденроллментлимит</span><span class="sxs-lookup"><span data-stu-id="b60da-103">suggestedEnrollmentLimit resource type</span></span>

<span data-ttu-id="b60da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b60da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b60da-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b60da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b60da-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b60da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b60da-107">Ресурс Сугжестеденроллментлимит представляет Рекомендуемое предельное значение регистрации при наличии типа регистрации.</span><span class="sxs-lookup"><span data-stu-id="b60da-107">The suggestedEnrollmentLimit resource represents the suggested enrollment limit when given an enrollment type.</span></span>

## <a name="properties"></a><span data-ttu-id="b60da-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b60da-108">Properties</span></span>
|<span data-ttu-id="b60da-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b60da-109">Property</span></span>|<span data-ttu-id="b60da-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b60da-110">Type</span></span>|<span data-ttu-id="b60da-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b60da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b60da-112">сугжестеддаилилимит</span><span class="sxs-lookup"><span data-stu-id="b60da-112">suggestedDailyLimit</span></span>|<span data-ttu-id="b60da-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b60da-113">Int32</span></span>|<span data-ttu-id="b60da-114">Предполагаемое количество заявок в течение дня</span><span class="sxs-lookup"><span data-stu-id="b60da-114">The suggested enrollment limit within a day</span></span>|

## <a name="relationships"></a><span data-ttu-id="b60da-115">Связи</span><span class="sxs-lookup"><span data-stu-id="b60da-115">Relationships</span></span>
<span data-ttu-id="b60da-116">Нет</span><span class="sxs-lookup"><span data-stu-id="b60da-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b60da-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b60da-117">JSON Representation</span></span>
<span data-ttu-id="b60da-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b60da-118">Here is a JSON representation of the resource.</span></span>
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






