---
title: тип списка appListType
description: Возможные значения списка приложений для соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2b8126ded9f6d0e9f68c6a9f5e8bcbcbbb216294
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755919"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="85acb-103">тип списка appListType</span><span class="sxs-lookup"><span data-stu-id="85acb-103">appListType enum type</span></span>

<span data-ttu-id="85acb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85acb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85acb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85acb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85acb-106">Возможные значения списка приложений для соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="85acb-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="85acb-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="85acb-107">Members</span></span>
|<span data-ttu-id="85acb-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="85acb-108">Member</span></span>|<span data-ttu-id="85acb-109">Значение</span><span class="sxs-lookup"><span data-stu-id="85acb-109">Value</span></span>|<span data-ttu-id="85acb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="85acb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85acb-111">нет</span><span class="sxs-lookup"><span data-stu-id="85acb-111">none</span></span>|<span data-ttu-id="85acb-112">0</span><span class="sxs-lookup"><span data-stu-id="85acb-112">0</span></span>|<span data-ttu-id="85acb-113">Значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="85acb-113">Default value, no intent.</span></span>|
|<span data-ttu-id="85acb-114">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="85acb-114">appsInListCompliant</span></span>|<span data-ttu-id="85acb-115">1</span><span class="sxs-lookup"><span data-stu-id="85acb-115">1</span></span>|<span data-ttu-id="85acb-116">В списке представлены приложения, которые будут считаться совместимыми (только приложения в списке совместимы).</span><span class="sxs-lookup"><span data-stu-id="85acb-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="85acb-117">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="85acb-117">appsNotInListCompliant</span></span>|<span data-ttu-id="85acb-118">2</span><span class="sxs-lookup"><span data-stu-id="85acb-118">2</span></span>|<span data-ttu-id="85acb-119">В списке представлены приложения, которые будут считаться не соответствующими требованиям (все приложения совместимы, за исключением приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="85acb-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




