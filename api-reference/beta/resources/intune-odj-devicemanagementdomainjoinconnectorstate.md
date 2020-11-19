---
title: тип перечисления Девицеманажементдомаинжоинконнекторстате
description: Состояние запроса ОДЖ.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 58b0a3a9e590913d0415062d6737fc6d9c33c451
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222760"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="a78ed-103">тип перечисления Девицеманажементдомаинжоинконнекторстате</span><span class="sxs-lookup"><span data-stu-id="a78ed-103">deviceManagementDomainJoinConnectorState enum type</span></span>

<span data-ttu-id="a78ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a78ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a78ed-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a78ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a78ed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a78ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a78ed-107">Состояние запроса ОДЖ.</span><span class="sxs-lookup"><span data-stu-id="a78ed-107">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="a78ed-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a78ed-108">Members</span></span>
|<span data-ttu-id="a78ed-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a78ed-109">Member</span></span>|<span data-ttu-id="a78ed-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a78ed-110">Value</span></span>|<span data-ttu-id="a78ed-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a78ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a78ed-112">ASP</span><span class="sxs-lookup"><span data-stu-id="a78ed-112">active</span></span>|<span data-ttu-id="a78ed-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a78ed-113">0</span></span>|<span data-ttu-id="a78ed-114">Соединитель активно проверяет связь с Intune.</span><span class="sxs-lookup"><span data-stu-id="a78ed-114">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="a78ed-115">error</span><span class="sxs-lookup"><span data-stu-id="a78ed-115">error</span></span>|<span data-ttu-id="a78ed-116">1,1</span><span class="sxs-lookup"><span data-stu-id="a78ed-116">1</span></span>|<span data-ttu-id="a78ed-117">Нет сердца-червей от последнего часа до 1 часа.</span><span class="sxs-lookup"><span data-stu-id="a78ed-117">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="a78ed-118">отсутств</span><span class="sxs-lookup"><span data-stu-id="a78ed-118">inactive</span></span>|<span data-ttu-id="a78ed-119">2</span><span class="sxs-lookup"><span data-stu-id="a78ed-119">2</span></span>|<span data-ttu-id="a78ed-120">От соединителя за последние 5 дней нет сердца-червей.</span><span class="sxs-lookup"><span data-stu-id="a78ed-120">There is no heart-beat from connector from last 5 days.</span></span>|




