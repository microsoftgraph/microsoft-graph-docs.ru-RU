---
title: тип перечисления Админконсентстате
description: Состояние согласия администратора.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0b7640cf2942d3f3ba9278effa8296585e4cd89f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528715"
---
# <a name="adminconsentstate-enum-type"></a><span data-ttu-id="7d40c-103">тип перечисления Админконсентстате</span><span class="sxs-lookup"><span data-stu-id="7d40c-103">adminConsentState enum type</span></span>

<span data-ttu-id="7d40c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7d40c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d40c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d40c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d40c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d40c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d40c-107">Состояние согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="7d40c-107">Admin consent state.</span></span>

## <a name="members"></a><span data-ttu-id="7d40c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="7d40c-108">Members</span></span>
|<span data-ttu-id="7d40c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="7d40c-109">Member</span></span>|<span data-ttu-id="7d40c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="7d40c-110">Value</span></span>|<span data-ttu-id="7d40c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7d40c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d40c-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7d40c-112">notConfigured</span></span>|<span data-ttu-id="7d40c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="7d40c-113">0</span></span>|<span data-ttu-id="7d40c-114">Администратор не настроил элемент</span><span class="sxs-lookup"><span data-stu-id="7d40c-114">Admin did not configure the item</span></span>|
|<span data-ttu-id="7d40c-115">granted</span><span class="sxs-lookup"><span data-stu-id="7d40c-115">granted</span></span>|<span data-ttu-id="7d40c-116">1 </span><span class="sxs-lookup"><span data-stu-id="7d40c-116">1</span></span>|<span data-ttu-id="7d40c-117">Элемент, которому назначен администратор</span><span class="sxs-lookup"><span data-stu-id="7d40c-117">Admin granted item</span></span>|
|<span data-ttu-id="7d40c-118">нотгрантед</span><span class="sxs-lookup"><span data-stu-id="7d40c-118">notGranted</span></span>|<span data-ttu-id="7d40c-119">2 </span><span class="sxs-lookup"><span data-stu-id="7d40c-119">2</span></span>|<span data-ttu-id="7d40c-120">Администратор не предоставляет элемент</span><span class="sxs-lookup"><span data-stu-id="7d40c-120">Admin does not grant item</span></span>|



