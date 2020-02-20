---
title: тип перечисления Глобалдевицехеалсскриптстате
description: Указывает, включены ли сценарии исправности глобальных устройств и находятся ли их в состоянии.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3f154e760398116ca6c22d21d6947c08a10e0eb4
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163824"
---
# <a name="globaldevicehealthscriptstate-enum-type"></a><span data-ttu-id="51a08-103">тип перечисления Глобалдевицехеалсскриптстате</span><span class="sxs-lookup"><span data-stu-id="51a08-103">globalDeviceHealthScriptState enum type</span></span>

> <span data-ttu-id="51a08-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51a08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51a08-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51a08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51a08-106">Указывает, включены ли сценарии исправности глобальных устройств и находятся ли их в состоянии.</span><span class="sxs-lookup"><span data-stu-id="51a08-106">Indicates whether global device health scripts are enabled and are in which state</span></span>

## <a name="members"></a><span data-ttu-id="51a08-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="51a08-107">Members</span></span>
|<span data-ttu-id="51a08-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="51a08-108">Member</span></span>|<span data-ttu-id="51a08-109">Значение</span><span class="sxs-lookup"><span data-stu-id="51a08-109">Value</span></span>|<span data-ttu-id="51a08-110">Описание</span><span class="sxs-lookup"><span data-stu-id="51a08-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51a08-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="51a08-111">notConfigured</span></span>|<span data-ttu-id="51a08-112">нуль</span><span class="sxs-lookup"><span data-stu-id="51a08-112">0</span></span>|<span data-ttu-id="51a08-113">Глобальные сценарии работоспособности устройств не настроены</span><span class="sxs-lookup"><span data-stu-id="51a08-113">Global device health scripts are not configured</span></span>|
|<span data-ttu-id="51a08-114">закончен</span><span class="sxs-lookup"><span data-stu-id="51a08-114">pending</span></span>|<span data-ttu-id="51a08-115">1,1</span><span class="sxs-lookup"><span data-stu-id="51a08-115">1</span></span>|<span data-ttu-id="51a08-116">Глобальные сценарии работоспособности устройств настроены, но не полностью включены</span><span class="sxs-lookup"><span data-stu-id="51a08-116">Global device health scripts are configured but not fully enabled</span></span>|
|<span data-ttu-id="51a08-117">enabled</span><span class="sxs-lookup"><span data-stu-id="51a08-117">enabled</span></span>|<span data-ttu-id="51a08-118">2</span><span class="sxs-lookup"><span data-stu-id="51a08-118">2</span></span>|<span data-ttu-id="51a08-119">Глобальные сценарии работоспособности устройств включены и готовы к использованию</span><span class="sxs-lookup"><span data-stu-id="51a08-119">Global device health scripts are enabled and ready to use</span></span>|



