---
title: тип enum vppTokenState
description: Возможные состояния, связанные с маркером Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 26492a317a5fe147a49cc8cda7103fa492704deb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755702"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="75a68-103">тип enum vppTokenState</span><span class="sxs-lookup"><span data-stu-id="75a68-103">vppTokenState enum type</span></span>

<span data-ttu-id="75a68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75a68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75a68-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75a68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75a68-106">Возможные состояния, связанные с маркером Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="75a68-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="75a68-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="75a68-107">Members</span></span>
|<span data-ttu-id="75a68-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="75a68-108">Member</span></span>|<span data-ttu-id="75a68-109">Значение</span><span class="sxs-lookup"><span data-stu-id="75a68-109">Value</span></span>|<span data-ttu-id="75a68-110">Описание</span><span class="sxs-lookup"><span data-stu-id="75a68-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75a68-111">unknown</span><span class="sxs-lookup"><span data-stu-id="75a68-111">unknown</span></span>|<span data-ttu-id="75a68-112">0</span><span class="sxs-lookup"><span data-stu-id="75a68-112">0</span></span>|<span data-ttu-id="75a68-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="75a68-113">Default state.</span></span>|
|<span data-ttu-id="75a68-114">допустимо</span><span class="sxs-lookup"><span data-stu-id="75a68-114">valid</span></span>|<span data-ttu-id="75a68-115">1</span><span class="sxs-lookup"><span data-stu-id="75a68-115">1</span></span>|<span data-ttu-id="75a68-116">Маркер действителен.</span><span class="sxs-lookup"><span data-stu-id="75a68-116">Token is valid.</span></span>|
|<span data-ttu-id="75a68-117">истек срок действия</span><span class="sxs-lookup"><span data-stu-id="75a68-117">expired</span></span>|<span data-ttu-id="75a68-118">2</span><span class="sxs-lookup"><span data-stu-id="75a68-118">2</span></span>|<span data-ttu-id="75a68-119">Срок действия маркера истек.</span><span class="sxs-lookup"><span data-stu-id="75a68-119">Token is expired.</span></span>|
|<span data-ttu-id="75a68-120">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="75a68-120">invalid</span></span>|<span data-ttu-id="75a68-121">3</span><span class="sxs-lookup"><span data-stu-id="75a68-121">3</span></span>|<span data-ttu-id="75a68-122">Маркер недействителен.</span><span class="sxs-lookup"><span data-stu-id="75a68-122">Token is invalid.</span></span>|
|<span data-ttu-id="75a68-123">назначеноToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="75a68-123">assignedToExternalMDM</span></span>|<span data-ttu-id="75a68-124">4 </span><span class="sxs-lookup"><span data-stu-id="75a68-124">4</span></span>|<span data-ttu-id="75a68-125">Маркер управляется другой службой MDM.</span><span class="sxs-lookup"><span data-stu-id="75a68-125">Token is managed by another MDM Service.</span></span>|




