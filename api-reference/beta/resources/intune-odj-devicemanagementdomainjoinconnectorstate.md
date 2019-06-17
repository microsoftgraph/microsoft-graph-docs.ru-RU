---
title: тип перечисления Девицеманажементдомаинжоинконнекторстате
description: Состояние запроса ОДЖ.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a584a77c0a921b9d5864270c5a42a9991123eb8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001918"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="6a31d-103">тип перечисления Девицеманажементдомаинжоинконнекторстате</span><span class="sxs-lookup"><span data-stu-id="6a31d-103">deviceManagementDomainJoinConnectorState enum type</span></span>

> <span data-ttu-id="6a31d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a31d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a31d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a31d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a31d-106">Состояние запроса ОДЖ.</span><span class="sxs-lookup"><span data-stu-id="6a31d-106">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="6a31d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="6a31d-107">Members</span></span>
|<span data-ttu-id="6a31d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="6a31d-108">Member</span></span>|<span data-ttu-id="6a31d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="6a31d-109">Value</span></span>|<span data-ttu-id="6a31d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6a31d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a31d-111">ASP</span><span class="sxs-lookup"><span data-stu-id="6a31d-111">active</span></span>|<span data-ttu-id="6a31d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="6a31d-112">0</span></span>|<span data-ttu-id="6a31d-113">Соединитель активно проверяет связь с Intune.</span><span class="sxs-lookup"><span data-stu-id="6a31d-113">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="6a31d-114">error</span><span class="sxs-lookup"><span data-stu-id="6a31d-114">error</span></span>|<span data-ttu-id="6a31d-115">1,1</span><span class="sxs-lookup"><span data-stu-id="6a31d-115">1</span></span>|<span data-ttu-id="6a31d-116">Нет сердца-червей от последнего часа до 1 часа.</span><span class="sxs-lookup"><span data-stu-id="6a31d-116">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="6a31d-117">отсутств</span><span class="sxs-lookup"><span data-stu-id="6a31d-117">inactive</span></span>|<span data-ttu-id="6a31d-118">2</span><span class="sxs-lookup"><span data-stu-id="6a31d-118">2</span></span>|<span data-ttu-id="6a31d-119">От соединителя за последние 5 дней нет сердца-червей.</span><span class="sxs-lookup"><span data-stu-id="6a31d-119">There is no heart-beat from connector from last 5 days.</span></span>|





