---
title: тип перечисления Глобалдевицехеалсскриптстате
description: Указывает, включены ли сценарии исправности глобальных устройств и находятся ли их в состоянии.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dbdcda672147c1e555727b9f5024744e287a6a6e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528577"
---
# <a name="globaldevicehealthscriptstate-enum-type"></a><span data-ttu-id="eb4b5-103">тип перечисления Глобалдевицехеалсскриптстате</span><span class="sxs-lookup"><span data-stu-id="eb4b5-103">globalDeviceHealthScriptState enum type</span></span>

<span data-ttu-id="eb4b5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eb4b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb4b5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb4b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb4b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb4b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb4b5-107">Указывает, включены ли сценарии исправности глобальных устройств и находятся ли их в состоянии.</span><span class="sxs-lookup"><span data-stu-id="eb4b5-107">Indicates whether global device health scripts are enabled and are in which state</span></span>

## <a name="members"></a><span data-ttu-id="eb4b5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="eb4b5-108">Members</span></span>
|<span data-ttu-id="eb4b5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="eb4b5-109">Member</span></span>|<span data-ttu-id="eb4b5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="eb4b5-110">Value</span></span>|<span data-ttu-id="eb4b5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eb4b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb4b5-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="eb4b5-112">notConfigured</span></span>|<span data-ttu-id="eb4b5-113">нуль</span><span class="sxs-lookup"><span data-stu-id="eb4b5-113">0</span></span>|<span data-ttu-id="eb4b5-114">Глобальные сценарии работоспособности устройств не настроены</span><span class="sxs-lookup"><span data-stu-id="eb4b5-114">Global device health scripts are not configured</span></span>|
|<span data-ttu-id="eb4b5-115">закончен</span><span class="sxs-lookup"><span data-stu-id="eb4b5-115">pending</span></span>|<span data-ttu-id="eb4b5-116">1 </span><span class="sxs-lookup"><span data-stu-id="eb4b5-116">1</span></span>|<span data-ttu-id="eb4b5-117">Глобальные сценарии работоспособности устройств настроены, но не полностью включены</span><span class="sxs-lookup"><span data-stu-id="eb4b5-117">Global device health scripts are configured but not fully enabled</span></span>|
|<span data-ttu-id="eb4b5-118">enabled</span><span class="sxs-lookup"><span data-stu-id="eb4b5-118">enabled</span></span>|<span data-ttu-id="eb4b5-119">2 </span><span class="sxs-lookup"><span data-stu-id="eb4b5-119">2</span></span>|<span data-ttu-id="eb4b5-120">Глобальные сценарии работоспособности устройств включены и готовы к использованию</span><span class="sxs-lookup"><span data-stu-id="eb4b5-120">Global device health scripts are enabled and ready to use</span></span>|



