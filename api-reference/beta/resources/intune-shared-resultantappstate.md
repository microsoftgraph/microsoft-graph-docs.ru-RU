---
title: тип перечисления Ресултантаппстате
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a4b50a903dc60e9f6d152c0b11f55811f85c446
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473531"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="4a556-103">тип перечисления Ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="4a556-103">resultantAppState enum type</span></span>

<span data-ttu-id="4a556-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a556-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a556-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a556-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a556-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a556-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a556-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4a556-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="4a556-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4a556-108">Members</span></span>
|<span data-ttu-id="4a556-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4a556-109">Member</span></span>|<span data-ttu-id="4a556-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4a556-110">Value</span></span>|<span data-ttu-id="4a556-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4a556-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a556-112">устанавлива</span><span class="sxs-lookup"><span data-stu-id="4a556-112">installed</span></span>|<span data-ttu-id="4a556-113">1,1</span><span class="sxs-lookup"><span data-stu-id="4a556-113">1</span></span>|<span data-ttu-id="4a556-114">Приложение установлено без ошибок</span><span class="sxs-lookup"><span data-stu-id="4a556-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="4a556-115">сбоев</span><span class="sxs-lookup"><span data-stu-id="4a556-115">failed</span></span>|<span data-ttu-id="4a556-116">2</span><span class="sxs-lookup"><span data-stu-id="4a556-116">2</span></span>|<span data-ttu-id="4a556-117">Не удалось установить приложение.</span><span class="sxs-lookup"><span data-stu-id="4a556-117">The application failed to install.</span></span>|
|<span data-ttu-id="4a556-118">нотинсталлед</span><span class="sxs-lookup"><span data-stu-id="4a556-118">notInstalled</span></span>|<span data-ttu-id="4a556-119">4</span><span class="sxs-lookup"><span data-stu-id="4a556-119">3</span></span>|<span data-ttu-id="4a556-120">Приложение не установлено.</span><span class="sxs-lookup"><span data-stu-id="4a556-120">The application is not installed.</span></span>|
|<span data-ttu-id="4a556-121">унинсталлфаилед</span><span class="sxs-lookup"><span data-stu-id="4a556-121">uninstallFailed</span></span>|<span data-ttu-id="4a556-122">4 </span><span class="sxs-lookup"><span data-stu-id="4a556-122">4</span></span>|<span data-ttu-id="4a556-123">Не удалось удалить приложение.</span><span class="sxs-lookup"><span data-stu-id="4a556-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="4a556-124">пендингинсталл</span><span class="sxs-lookup"><span data-stu-id="4a556-124">pendingInstall</span></span>|<span data-ttu-id="4a556-125">5 </span><span class="sxs-lookup"><span data-stu-id="4a556-125">5</span></span>|<span data-ttu-id="4a556-126">Выполняется установка приложения.</span><span class="sxs-lookup"><span data-stu-id="4a556-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="4a556-127">unknown</span><span class="sxs-lookup"><span data-stu-id="4a556-127">unknown</span></span>|<span data-ttu-id="4a556-128">99</span><span class="sxs-lookup"><span data-stu-id="4a556-128">99</span></span>|<span data-ttu-id="4a556-129">Неизвестное состояние приложения.</span><span class="sxs-lookup"><span data-stu-id="4a556-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="4a556-130">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="4a556-130">notApplicable</span></span>|<span data-ttu-id="4a556-131">–1</span><span class="sxs-lookup"><span data-stu-id="4a556-131">-1</span></span>|<span data-ttu-id="4a556-132">Приложение неприменимо.</span><span class="sxs-lookup"><span data-stu-id="4a556-132">The application is not applicable.</span></span>|



