---
title: Тип перечисления mobileAppPublishingState
description: Указывает состояние публикации приложения.
author: tfitzmac
ms.openlocfilehash: 2415e2ba244d7766cbdc670c303643ec125c1091
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302333"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="03989-103">Тип перечисления mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="03989-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="03989-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="03989-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03989-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03989-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03989-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="03989-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03989-107">Указывает состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="03989-107">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="03989-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="03989-108">Members</span></span>
|<span data-ttu-id="03989-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="03989-109">Member</span></span>|<span data-ttu-id="03989-110">Значение</span><span class="sxs-lookup"><span data-stu-id="03989-110">Value</span></span>|<span data-ttu-id="03989-111">Описание</span><span class="sxs-lookup"><span data-stu-id="03989-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03989-112">notPublished</span><span class="sxs-lookup"><span data-stu-id="03989-112">notPublished</span></span>|<span data-ttu-id="03989-113">0</span><span class="sxs-lookup"><span data-stu-id="03989-113">0</span></span>|<span data-ttu-id="03989-114">Приложение не публикуется.</span><span class="sxs-lookup"><span data-stu-id="03989-114">The app is not yet published.</span></span>|
|<span data-ttu-id="03989-115">обработка</span><span class="sxs-lookup"><span data-stu-id="03989-115">processing</span></span>|<span data-ttu-id="03989-116">1</span><span class="sxs-lookup"><span data-stu-id="03989-116">1</span></span>|<span data-ttu-id="03989-117">Приложение ожидает обработки на стороне службы.</span><span class="sxs-lookup"><span data-stu-id="03989-117">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="03989-118">опубликованный</span><span class="sxs-lookup"><span data-stu-id="03989-118">published</span></span>|<span data-ttu-id="03989-119">2</span><span class="sxs-lookup"><span data-stu-id="03989-119">2</span></span>|<span data-ttu-id="03989-120">Приложение будет опубликовано.</span><span class="sxs-lookup"><span data-stu-id="03989-120">The app is published.</span></span>|





