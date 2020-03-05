---
title: тип перечисления Девицеманажементдомаинжоинконнекторстате
description: Состояние запроса ОДЖ.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9cee18df0fe6ba3cc59d8d427aa472f8943e03d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527795"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="4551d-103">тип перечисления Девицеманажементдомаинжоинконнекторстате</span><span class="sxs-lookup"><span data-stu-id="4551d-103">deviceManagementDomainJoinConnectorState enum type</span></span>

<span data-ttu-id="4551d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4551d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4551d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4551d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4551d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4551d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4551d-107">Состояние запроса ОДЖ.</span><span class="sxs-lookup"><span data-stu-id="4551d-107">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="4551d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4551d-108">Members</span></span>
|<span data-ttu-id="4551d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4551d-109">Member</span></span>|<span data-ttu-id="4551d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4551d-110">Value</span></span>|<span data-ttu-id="4551d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4551d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4551d-112">ASP</span><span class="sxs-lookup"><span data-stu-id="4551d-112">active</span></span>|<span data-ttu-id="4551d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="4551d-113">0</span></span>|<span data-ttu-id="4551d-114">Соединитель активно проверяет связь с Intune.</span><span class="sxs-lookup"><span data-stu-id="4551d-114">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="4551d-115">error</span><span class="sxs-lookup"><span data-stu-id="4551d-115">error</span></span>|<span data-ttu-id="4551d-116">1 </span><span class="sxs-lookup"><span data-stu-id="4551d-116">1</span></span>|<span data-ttu-id="4551d-117">Нет сердца-червей от последнего часа до 1 часа.</span><span class="sxs-lookup"><span data-stu-id="4551d-117">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="4551d-118">отсутств</span><span class="sxs-lookup"><span data-stu-id="4551d-118">inactive</span></span>|<span data-ttu-id="4551d-119">2 </span><span class="sxs-lookup"><span data-stu-id="4551d-119">2</span></span>|<span data-ttu-id="4551d-120">От соединителя за последние 5 дней нет сердца-червей.</span><span class="sxs-lookup"><span data-stu-id="4551d-120">There is no heart-beat from connector from last 5 days.</span></span>|



