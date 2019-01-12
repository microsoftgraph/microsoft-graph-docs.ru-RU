---
title: Тип перечисления mobileAppPublishingState
description: Указывает состояние публикации приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 270dd416422c0f0b4dfc320937c749f4fe13c766
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937763"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="872f7-103">Тип перечисления mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="872f7-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="872f7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="872f7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="872f7-105">Указывает состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="872f7-105">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="872f7-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="872f7-106">Members</span></span>
|<span data-ttu-id="872f7-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="872f7-107">Member</span></span>|<span data-ttu-id="872f7-108">Значение</span><span class="sxs-lookup"><span data-stu-id="872f7-108">Value</span></span>|<span data-ttu-id="872f7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="872f7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="872f7-110">notPublished</span><span class="sxs-lookup"><span data-stu-id="872f7-110">notPublished</span></span>|<span data-ttu-id="872f7-111">0</span><span class="sxs-lookup"><span data-stu-id="872f7-111">0</span></span>|<span data-ttu-id="872f7-112">Приложение не публикуется.</span><span class="sxs-lookup"><span data-stu-id="872f7-112">The app is not yet published.</span></span>|
|<span data-ttu-id="872f7-113">обработка</span><span class="sxs-lookup"><span data-stu-id="872f7-113">processing</span></span>|<span data-ttu-id="872f7-114">1</span><span class="sxs-lookup"><span data-stu-id="872f7-114">1</span></span>|<span data-ttu-id="872f7-115">Приложение ожидает обработки на стороне службы.</span><span class="sxs-lookup"><span data-stu-id="872f7-115">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="872f7-116">опубликованный</span><span class="sxs-lookup"><span data-stu-id="872f7-116">published</span></span>|<span data-ttu-id="872f7-117">2</span><span class="sxs-lookup"><span data-stu-id="872f7-117">2</span></span>|<span data-ttu-id="872f7-118">Приложение будет опубликовано.</span><span class="sxs-lookup"><span data-stu-id="872f7-118">The app is published.</span></span>|



