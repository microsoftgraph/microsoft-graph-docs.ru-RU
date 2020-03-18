---
title: тип перечисления Девицеманажементдомаинжоинконнекторстате
description: Состояние запроса ОДЖ.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e8eff02a8ff4d47f920bad6506bcb9e3b37f0785
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779886"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="3c1f9-103">тип перечисления Девицеманажементдомаинжоинконнекторстате</span><span class="sxs-lookup"><span data-stu-id="3c1f9-103">deviceManagementDomainJoinConnectorState enum type</span></span>

> <span data-ttu-id="3c1f9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c1f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c1f9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c1f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c1f9-106">Состояние запроса ОДЖ.</span><span class="sxs-lookup"><span data-stu-id="3c1f9-106">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="3c1f9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3c1f9-107">Members</span></span>
|<span data-ttu-id="3c1f9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3c1f9-108">Member</span></span>|<span data-ttu-id="3c1f9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3c1f9-109">Value</span></span>|<span data-ttu-id="3c1f9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3c1f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c1f9-111">ASP</span><span class="sxs-lookup"><span data-stu-id="3c1f9-111">active</span></span>|<span data-ttu-id="3c1f9-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3c1f9-112">0</span></span>|<span data-ttu-id="3c1f9-113">Соединитель активно проверяет связь с Intune.</span><span class="sxs-lookup"><span data-stu-id="3c1f9-113">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="3c1f9-114">error</span><span class="sxs-lookup"><span data-stu-id="3c1f9-114">error</span></span>|<span data-ttu-id="3c1f9-115">1,1</span><span class="sxs-lookup"><span data-stu-id="3c1f9-115">1</span></span>|<span data-ttu-id="3c1f9-116">Нет сердца-червей от последнего часа до 1 часа.</span><span class="sxs-lookup"><span data-stu-id="3c1f9-116">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="3c1f9-117">отсутств</span><span class="sxs-lookup"><span data-stu-id="3c1f9-117">inactive</span></span>|<span data-ttu-id="3c1f9-118">2</span><span class="sxs-lookup"><span data-stu-id="3c1f9-118">2</span></span>|<span data-ttu-id="3c1f9-119">От соединителя за последние 5 дней нет сердца-червей.</span><span class="sxs-lookup"><span data-stu-id="3c1f9-119">There is no heart-beat from connector from last 5 days.</span></span>|



