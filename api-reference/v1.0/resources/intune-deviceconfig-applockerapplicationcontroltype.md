---
title: тип enum appLockerApplicationControlType
description: Возможные значения типов управления приложениями AppLocker
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 77a47a2654c8e585cadcf48d375d29eedd470991
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755912"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="f16eb-103">тип enum appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="f16eb-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="f16eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f16eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f16eb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f16eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f16eb-106">Возможные значения типов управления приложениями AppLocker</span><span class="sxs-lookup"><span data-stu-id="f16eb-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="f16eb-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f16eb-107">Members</span></span>
|<span data-ttu-id="f16eb-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f16eb-108">Member</span></span>|<span data-ttu-id="f16eb-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f16eb-109">Value</span></span>|<span data-ttu-id="f16eb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f16eb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f16eb-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f16eb-111">notConfigured</span></span>|<span data-ttu-id="f16eb-112">0</span><span class="sxs-lookup"><span data-stu-id="f16eb-112">0</span></span>|<span data-ttu-id="f16eb-113">Значение устройства по умолчанию, не выбранный тип управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="f16eb-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="f16eb-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="f16eb-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="f16eb-115">1</span><span class="sxs-lookup"><span data-stu-id="f16eb-115">1</span></span>|<span data-ttu-id="f16eb-116">Обеспечение Windows компонентов и хранения приложений.</span><span class="sxs-lookup"><span data-stu-id="f16eb-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="f16eb-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="f16eb-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="f16eb-118">2</span><span class="sxs-lookup"><span data-stu-id="f16eb-118">2</span></span>|<span data-ttu-id="f16eb-119">Аудит Windows компонентов и хранения приложений.</span><span class="sxs-lookup"><span data-stu-id="f16eb-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="f16eb-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="f16eb-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="f16eb-121">3</span><span class="sxs-lookup"><span data-stu-id="f16eb-121">3</span></span>|<span data-ttu-id="f16eb-122">Обеспечение Windows компонентов, хранения приложений и смарт-шкафчик.</span><span class="sxs-lookup"><span data-stu-id="f16eb-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="f16eb-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="f16eb-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="f16eb-124">4 </span><span class="sxs-lookup"><span data-stu-id="f16eb-124">4</span></span>|<span data-ttu-id="f16eb-125">Аудит Windows компонентов, хранения приложений и смарт-шкафчик.</span><span class="sxs-lookup"><span data-stu-id="f16eb-125">Audit Windows components, store apps and smart locker.</span></span>|




