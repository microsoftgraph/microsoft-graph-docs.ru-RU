---
title: тип перечисления Глобалдевицехеалсскриптстате
description: Указывает, включены ли сценарии исправности глобальных устройств и находятся ли их в состоянии.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0f838b252b53158724166a2d189fecfbfdf492c8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784042"
---
# <a name="globaldevicehealthscriptstate-enum-type"></a><span data-ttu-id="99588-103">тип перечисления Глобалдевицехеалсскриптстате</span><span class="sxs-lookup"><span data-stu-id="99588-103">globalDeviceHealthScriptState enum type</span></span>

> <span data-ttu-id="99588-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99588-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99588-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99588-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99588-106">Указывает, включены ли сценарии исправности глобальных устройств и находятся ли их в состоянии.</span><span class="sxs-lookup"><span data-stu-id="99588-106">Indicates whether global device health scripts are enabled and are in which state</span></span>

## <a name="members"></a><span data-ttu-id="99588-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="99588-107">Members</span></span>
|<span data-ttu-id="99588-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="99588-108">Member</span></span>|<span data-ttu-id="99588-109">Значение</span><span class="sxs-lookup"><span data-stu-id="99588-109">Value</span></span>|<span data-ttu-id="99588-110">Описание</span><span class="sxs-lookup"><span data-stu-id="99588-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99588-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="99588-111">notConfigured</span></span>|<span data-ttu-id="99588-112">нуль</span><span class="sxs-lookup"><span data-stu-id="99588-112">0</span></span>|<span data-ttu-id="99588-113">Глобальные сценарии работоспособности устройств не настроены</span><span class="sxs-lookup"><span data-stu-id="99588-113">Global device health scripts are not configured</span></span>|
|<span data-ttu-id="99588-114">закончен</span><span class="sxs-lookup"><span data-stu-id="99588-114">pending</span></span>|<span data-ttu-id="99588-115">1,1</span><span class="sxs-lookup"><span data-stu-id="99588-115">1</span></span>|<span data-ttu-id="99588-116">Глобальные сценарии работоспособности устройств настроены, но не полностью включены</span><span class="sxs-lookup"><span data-stu-id="99588-116">Global device health scripts are configured but not fully enabled</span></span>|
|<span data-ttu-id="99588-117">enabled</span><span class="sxs-lookup"><span data-stu-id="99588-117">enabled</span></span>|<span data-ttu-id="99588-118">2</span><span class="sxs-lookup"><span data-stu-id="99588-118">2</span></span>|<span data-ttu-id="99588-119">Глобальные сценарии работоспособности устройств включены и готовы к использованию</span><span class="sxs-lookup"><span data-stu-id="99588-119">Global device health scripts are enabled and ready to use</span></span>|



