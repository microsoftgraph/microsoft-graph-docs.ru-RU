---
title: тип перечисления Глобалдевицехеалсскриптстате
description: Указывает, включены ли сценарии исправности глобальных устройств и находятся ли их в состоянии.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e9b1ca70ca5c9d30d515b4d20bd27525249806fe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470651"
---
# <a name="globaldevicehealthscriptstate-enum-type"></a><span data-ttu-id="013aa-103">тип перечисления Глобалдевицехеалсскриптстате</span><span class="sxs-lookup"><span data-stu-id="013aa-103">globalDeviceHealthScriptState enum type</span></span>

<span data-ttu-id="013aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="013aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="013aa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="013aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="013aa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="013aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="013aa-107">Указывает, включены ли сценарии исправности глобальных устройств и находятся ли их в состоянии.</span><span class="sxs-lookup"><span data-stu-id="013aa-107">Indicates whether global device health scripts are enabled and are in which state</span></span>

## <a name="members"></a><span data-ttu-id="013aa-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="013aa-108">Members</span></span>
|<span data-ttu-id="013aa-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="013aa-109">Member</span></span>|<span data-ttu-id="013aa-110">Значение</span><span class="sxs-lookup"><span data-stu-id="013aa-110">Value</span></span>|<span data-ttu-id="013aa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="013aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="013aa-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="013aa-112">notConfigured</span></span>|<span data-ttu-id="013aa-113">нуль</span><span class="sxs-lookup"><span data-stu-id="013aa-113">0</span></span>|<span data-ttu-id="013aa-114">Глобальные сценарии работоспособности устройств не настроены</span><span class="sxs-lookup"><span data-stu-id="013aa-114">Global device health scripts are not configured</span></span>|
|<span data-ttu-id="013aa-115">закончен</span><span class="sxs-lookup"><span data-stu-id="013aa-115">pending</span></span>|<span data-ttu-id="013aa-116">1,1</span><span class="sxs-lookup"><span data-stu-id="013aa-116">1</span></span>|<span data-ttu-id="013aa-117">Глобальные сценарии работоспособности устройств настроены, но не полностью включены</span><span class="sxs-lookup"><span data-stu-id="013aa-117">Global device health scripts are configured but not fully enabled</span></span>|
|<span data-ttu-id="013aa-118">включено</span><span class="sxs-lookup"><span data-stu-id="013aa-118">enabled</span></span>|<span data-ttu-id="013aa-119">2</span><span class="sxs-lookup"><span data-stu-id="013aa-119">2</span></span>|<span data-ttu-id="013aa-120">Глобальные сценарии работоспособности устройств включены и готовы к использованию</span><span class="sxs-lookup"><span data-stu-id="013aa-120">Global device health scripts are enabled and ready to use</span></span>|



