---
title: Тип перечисления appListType
description: Возможные значения список соответствия требованиям приложения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf8930136b00b7b5579ec5e7266b6a77a9a11968
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415224"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="39da0-103">Тип перечисления appListType</span><span class="sxs-lookup"><span data-stu-id="39da0-103">appListType enum type</span></span>

> <span data-ttu-id="39da0-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="39da0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="39da0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39da0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39da0-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39da0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39da0-107">Возможные значения список соответствия требованиям приложения.</span><span class="sxs-lookup"><span data-stu-id="39da0-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="39da0-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="39da0-108">Members</span></span>
|<span data-ttu-id="39da0-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="39da0-109">Member</span></span>|<span data-ttu-id="39da0-110">Значение</span><span class="sxs-lookup"><span data-stu-id="39da0-110">Value</span></span>|<span data-ttu-id="39da0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="39da0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39da0-112">none</span><span class="sxs-lookup"><span data-stu-id="39da0-112">none</span></span>|<span data-ttu-id="39da0-113">0</span><span class="sxs-lookup"><span data-stu-id="39da0-113">0</span></span>|<span data-ttu-id="39da0-114">Значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="39da0-114">Default value, no intent.</span></span>|
|<span data-ttu-id="39da0-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="39da0-115">appsInListCompliant</span></span>|<span data-ttu-id="39da0-116">1</span><span class="sxs-lookup"><span data-stu-id="39da0-116">1</span></span>|<span data-ttu-id="39da0-117">Список представляет приложений, которые будут считаться спецификации (только для приложений в списке совместимых).</span><span class="sxs-lookup"><span data-stu-id="39da0-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="39da0-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="39da0-118">appsNotInListCompliant</span></span>|<span data-ttu-id="39da0-119">2</span><span class="sxs-lookup"><span data-stu-id="39da0-119">2</span></span>|<span data-ttu-id="39da0-120">Представляет список приложений, которые будут считаться несовместимой (все приложения совместимых за исключением приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="39da0-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




