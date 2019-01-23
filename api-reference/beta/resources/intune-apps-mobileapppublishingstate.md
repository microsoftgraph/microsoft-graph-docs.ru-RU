---
title: Тип перечисления mobileAppPublishingState
description: Указывает состояние публикации приложения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: db10e62e714e50ccdf9bac933b2746cb52ea25eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423883"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="e57c9-103">Тип перечисления mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e57c9-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="e57c9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e57c9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e57c9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e57c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e57c9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e57c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e57c9-107">Указывает состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="e57c9-107">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="e57c9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e57c9-108">Members</span></span>
|<span data-ttu-id="e57c9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e57c9-109">Member</span></span>|<span data-ttu-id="e57c9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e57c9-110">Value</span></span>|<span data-ttu-id="e57c9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e57c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e57c9-112">notPublished</span><span class="sxs-lookup"><span data-stu-id="e57c9-112">notPublished</span></span>|<span data-ttu-id="e57c9-113">0</span><span class="sxs-lookup"><span data-stu-id="e57c9-113">0</span></span>|<span data-ttu-id="e57c9-114">Приложение не публикуется.</span><span class="sxs-lookup"><span data-stu-id="e57c9-114">The app is not yet published.</span></span>|
|<span data-ttu-id="e57c9-115">обработка</span><span class="sxs-lookup"><span data-stu-id="e57c9-115">processing</span></span>|<span data-ttu-id="e57c9-116">1</span><span class="sxs-lookup"><span data-stu-id="e57c9-116">1</span></span>|<span data-ttu-id="e57c9-117">Приложение ожидает обработки на стороне службы.</span><span class="sxs-lookup"><span data-stu-id="e57c9-117">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="e57c9-118">опубликованный</span><span class="sxs-lookup"><span data-stu-id="e57c9-118">published</span></span>|<span data-ttu-id="e57c9-119">2</span><span class="sxs-lookup"><span data-stu-id="e57c9-119">2</span></span>|<span data-ttu-id="e57c9-120">Приложение будет опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e57c9-120">The app is published.</span></span>|




