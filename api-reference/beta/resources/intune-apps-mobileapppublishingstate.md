---
title: Тип перечисления mobileAppPublishingState
description: Указывает состояние публикации приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6b2ae893a0c971bfa0a80a09bb8e7c80b6146555
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932821"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="31422-103">Тип перечисления mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="31422-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="31422-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="31422-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31422-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31422-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31422-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="31422-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31422-107">Указывает состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="31422-107">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="31422-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="31422-108">Members</span></span>
|<span data-ttu-id="31422-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="31422-109">Member</span></span>|<span data-ttu-id="31422-110">Значение</span><span class="sxs-lookup"><span data-stu-id="31422-110">Value</span></span>|<span data-ttu-id="31422-111">Описание</span><span class="sxs-lookup"><span data-stu-id="31422-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31422-112">notPublished</span><span class="sxs-lookup"><span data-stu-id="31422-112">notPublished</span></span>|<span data-ttu-id="31422-113">0</span><span class="sxs-lookup"><span data-stu-id="31422-113">0</span></span>|<span data-ttu-id="31422-114">Приложение не публикуется.</span><span class="sxs-lookup"><span data-stu-id="31422-114">The app is not yet published.</span></span>|
|<span data-ttu-id="31422-115">обработка</span><span class="sxs-lookup"><span data-stu-id="31422-115">processing</span></span>|<span data-ttu-id="31422-116">1</span><span class="sxs-lookup"><span data-stu-id="31422-116">1</span></span>|<span data-ttu-id="31422-117">Приложение ожидает обработки на стороне службы.</span><span class="sxs-lookup"><span data-stu-id="31422-117">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="31422-118">опубликованный</span><span class="sxs-lookup"><span data-stu-id="31422-118">published</span></span>|<span data-ttu-id="31422-119">2</span><span class="sxs-lookup"><span data-stu-id="31422-119">2</span></span>|<span data-ttu-id="31422-120">Приложение будет опубликовано.</span><span class="sxs-lookup"><span data-stu-id="31422-120">The app is published.</span></span>|





