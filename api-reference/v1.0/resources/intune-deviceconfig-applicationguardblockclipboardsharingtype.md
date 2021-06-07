---
title: тип enum applicationGuardBlockClipboardSharingType
description: Возможные значения для приложенияGuardBlockClipboardSharingType
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a70f654c283a32db4e89ccc1b3991ffba49fc89e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755940"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="57003-103">тип enum applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="57003-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="57003-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57003-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57003-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57003-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57003-106">Возможные значения для приложенияGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="57003-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="57003-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="57003-107">Members</span></span>
|<span data-ttu-id="57003-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="57003-108">Member</span></span>|<span data-ttu-id="57003-109">Значение</span><span class="sxs-lookup"><span data-stu-id="57003-109">Value</span></span>|<span data-ttu-id="57003-110">Описание</span><span class="sxs-lookup"><span data-stu-id="57003-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57003-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="57003-111">notConfigured</span></span>|<span data-ttu-id="57003-112">0</span><span class="sxs-lookup"><span data-stu-id="57003-112">0</span></span>|<span data-ttu-id="57003-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="57003-113">Not Configured</span></span>|
|<span data-ttu-id="57003-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="57003-114">blockBoth</span></span>|<span data-ttu-id="57003-115">1</span><span class="sxs-lookup"><span data-stu-id="57003-115">1</span></span>|<span data-ttu-id="57003-116">Блокировка буфера обмена данными как от хоста до контейнера, так и от контейнера к хосту</span><span class="sxs-lookup"><span data-stu-id="57003-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="57003-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="57003-117">blockHostToContainer</span></span>|<span data-ttu-id="57003-118">2</span><span class="sxs-lookup"><span data-stu-id="57003-118">2</span></span>|<span data-ttu-id="57003-119">Блокировка буфера обмена данными с хост-контейнера</span><span class="sxs-lookup"><span data-stu-id="57003-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="57003-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="57003-120">blockContainerToHost</span></span>|<span data-ttu-id="57003-121">3</span><span class="sxs-lookup"><span data-stu-id="57003-121">3</span></span>|<span data-ttu-id="57003-122">Блокировка буфера обмена данными из контейнера в хост</span><span class="sxs-lookup"><span data-stu-id="57003-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="57003-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="57003-123">blockNone</span></span>|<span data-ttu-id="57003-124">4 </span><span class="sxs-lookup"><span data-stu-id="57003-124">4</span></span>|<span data-ttu-id="57003-125">Блокировка буфера обмена данными ни от хоста до контейнера, ни от контейнера к хосту</span><span class="sxs-lookup"><span data-stu-id="57003-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|




