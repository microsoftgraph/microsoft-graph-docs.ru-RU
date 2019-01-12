---
title: Тип перечисления edgeCookiePolicy
description: Возможные значения, чтобы указать, какие файлы cookie разрешены в Microsoft пограничного сервера.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 268f58cefcf4e43ecdac1191b67a9d242c17d624
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982157"
---
# <a name="edgecookiepolicy-enum-type"></a><span data-ttu-id="0a6a9-103">Тип перечисления edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="0a6a9-103">edgeCookiePolicy enum type</span></span>

> <span data-ttu-id="0a6a9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a6a9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a6a9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a6a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a6a9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0a6a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a6a9-107">Возможные значения, чтобы указать, какие файлы cookie разрешены в Microsoft пограничного сервера.</span><span class="sxs-lookup"><span data-stu-id="0a6a9-107">Possible values to specify which cookies are allowed in Microsoft Edge.</span></span>
## <a name="members"></a><span data-ttu-id="0a6a9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0a6a9-108">Members</span></span>
|<span data-ttu-id="0a6a9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0a6a9-109">Member</span></span>|<span data-ttu-id="0a6a9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0a6a9-110">Value</span></span>|<span data-ttu-id="0a6a9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a6a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a6a9-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="0a6a9-112">userDefined</span></span>|<span data-ttu-id="0a6a9-113">0</span><span class="sxs-lookup"><span data-stu-id="0a6a9-113">0</span></span>|<span data-ttu-id="0a6a9-114">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="0a6a9-114">Allow the user to set.</span></span>|
|<span data-ttu-id="0a6a9-115">Разрешить</span><span class="sxs-lookup"><span data-stu-id="0a6a9-115">allow</span></span>|<span data-ttu-id="0a6a9-116">1</span><span class="sxs-lookup"><span data-stu-id="0a6a9-116">1</span></span>|<span data-ttu-id="0a6a9-117">Разрешить.</span><span class="sxs-lookup"><span data-stu-id="0a6a9-117">Allow.</span></span>|
|<span data-ttu-id="0a6a9-118">blockThirdParty</span><span class="sxs-lookup"><span data-stu-id="0a6a9-118">blockThirdParty</span></span>|<span data-ttu-id="0a6a9-119">2</span><span class="sxs-lookup"><span data-stu-id="0a6a9-119">2</span></span>|<span data-ttu-id="0a6a9-120">Блокировать только файлы cookie сторонних производителей.</span><span class="sxs-lookup"><span data-stu-id="0a6a9-120">Block only third party cookies.</span></span>|
|<span data-ttu-id="0a6a9-121">blockAll</span><span class="sxs-lookup"><span data-stu-id="0a6a9-121">blockAll</span></span>|<span data-ttu-id="0a6a9-122">3</span><span class="sxs-lookup"><span data-stu-id="0a6a9-122">3</span></span>|<span data-ttu-id="0a6a9-123">Блокировать все файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="0a6a9-123">Block all cookies.</span></span>|





