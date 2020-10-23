---
title: тип перечисления Ресултантаппстате
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b431a4ca3b44afc54547e3dc7e02e1886c95618a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730341"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="2c248-103">тип перечисления Ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="2c248-103">resultantAppState enum type</span></span>

<span data-ttu-id="2c248-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c248-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c248-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c248-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c248-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c248-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c248-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2c248-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="2c248-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2c248-108">Members</span></span>
|<span data-ttu-id="2c248-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2c248-109">Member</span></span>|<span data-ttu-id="2c248-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2c248-110">Value</span></span>|<span data-ttu-id="2c248-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2c248-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c248-112">устанавлива</span><span class="sxs-lookup"><span data-stu-id="2c248-112">installed</span></span>|<span data-ttu-id="2c248-113">1,1</span><span class="sxs-lookup"><span data-stu-id="2c248-113">1</span></span>|<span data-ttu-id="2c248-114">Приложение установлено без ошибок</span><span class="sxs-lookup"><span data-stu-id="2c248-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="2c248-115">сбоев</span><span class="sxs-lookup"><span data-stu-id="2c248-115">failed</span></span>|<span data-ttu-id="2c248-116">2</span><span class="sxs-lookup"><span data-stu-id="2c248-116">2</span></span>|<span data-ttu-id="2c248-117">Не удалось установить приложение.</span><span class="sxs-lookup"><span data-stu-id="2c248-117">The application failed to install.</span></span>|
|<span data-ttu-id="2c248-118">нотинсталлед</span><span class="sxs-lookup"><span data-stu-id="2c248-118">notInstalled</span></span>|<span data-ttu-id="2c248-119">4</span><span class="sxs-lookup"><span data-stu-id="2c248-119">3</span></span>|<span data-ttu-id="2c248-120">Приложение не установлено.</span><span class="sxs-lookup"><span data-stu-id="2c248-120">The application is not installed.</span></span>|
|<span data-ttu-id="2c248-121">унинсталлфаилед</span><span class="sxs-lookup"><span data-stu-id="2c248-121">uninstallFailed</span></span>|<span data-ttu-id="2c248-122">4 </span><span class="sxs-lookup"><span data-stu-id="2c248-122">4</span></span>|<span data-ttu-id="2c248-123">Не удалось удалить приложение.</span><span class="sxs-lookup"><span data-stu-id="2c248-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="2c248-124">пендингинсталл</span><span class="sxs-lookup"><span data-stu-id="2c248-124">pendingInstall</span></span>|<span data-ttu-id="2c248-125">5 </span><span class="sxs-lookup"><span data-stu-id="2c248-125">5</span></span>|<span data-ttu-id="2c248-126">Выполняется установка приложения.</span><span class="sxs-lookup"><span data-stu-id="2c248-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="2c248-127">unknown</span><span class="sxs-lookup"><span data-stu-id="2c248-127">unknown</span></span>|<span data-ttu-id="2c248-128">99</span><span class="sxs-lookup"><span data-stu-id="2c248-128">99</span></span>|<span data-ttu-id="2c248-129">Неизвестное состояние приложения.</span><span class="sxs-lookup"><span data-stu-id="2c248-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="2c248-130">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="2c248-130">notApplicable</span></span>|<span data-ttu-id="2c248-131">–1</span><span class="sxs-lookup"><span data-stu-id="2c248-131">-1</span></span>|<span data-ttu-id="2c248-132">Приложение неприменимо.</span><span class="sxs-lookup"><span data-stu-id="2c248-132">The application is not applicable.</span></span>|





