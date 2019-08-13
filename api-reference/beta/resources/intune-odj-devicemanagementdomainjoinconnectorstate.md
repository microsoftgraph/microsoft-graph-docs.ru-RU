---
title: тип перечисления Девицеманажементдомаинжоинконнекторстате
description: Состояние запроса ОДЖ.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f664a6b57d92f5a8cd2d586f8bc2747ffa6db71c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342007"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="c045b-103">тип перечисления Девицеманажементдомаинжоинконнекторстате</span><span class="sxs-lookup"><span data-stu-id="c045b-103">deviceManagementDomainJoinConnectorState enum type</span></span>

> <span data-ttu-id="c045b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c045b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c045b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c045b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c045b-106">Состояние запроса ОДЖ.</span><span class="sxs-lookup"><span data-stu-id="c045b-106">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="c045b-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c045b-107">Members</span></span>
|<span data-ttu-id="c045b-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c045b-108">Member</span></span>|<span data-ttu-id="c045b-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c045b-109">Value</span></span>|<span data-ttu-id="c045b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c045b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c045b-111">ASP</span><span class="sxs-lookup"><span data-stu-id="c045b-111">active</span></span>|<span data-ttu-id="c045b-112">нуль</span><span class="sxs-lookup"><span data-stu-id="c045b-112">0</span></span>|<span data-ttu-id="c045b-113">Соединитель активно проверяет связь с Intune.</span><span class="sxs-lookup"><span data-stu-id="c045b-113">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="c045b-114">error</span><span class="sxs-lookup"><span data-stu-id="c045b-114">error</span></span>|<span data-ttu-id="c045b-115">1,1</span><span class="sxs-lookup"><span data-stu-id="c045b-115">1</span></span>|<span data-ttu-id="c045b-116">Нет сердца-червей от последнего часа до 1 часа.</span><span class="sxs-lookup"><span data-stu-id="c045b-116">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="c045b-117">отсутств</span><span class="sxs-lookup"><span data-stu-id="c045b-117">inactive</span></span>|<span data-ttu-id="c045b-118">2</span><span class="sxs-lookup"><span data-stu-id="c045b-118">2</span></span>|<span data-ttu-id="c045b-119">От соединителя за последние 5 дней нет сердца-червей.</span><span class="sxs-lookup"><span data-stu-id="c045b-119">There is no heart-beat from connector from last 5 days.</span></span>|



