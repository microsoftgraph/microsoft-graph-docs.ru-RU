---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 172908882d6a9efd03d9645e8a562a70622fea12
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795921"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="b8206-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="b8206-103">appListType enum type</span></span>

> <span data-ttu-id="b8206-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8206-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8206-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8206-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8206-106">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="b8206-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="b8206-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b8206-107">Members</span></span>
|<span data-ttu-id="b8206-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b8206-108">Member</span></span>|<span data-ttu-id="b8206-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b8206-109">Value</span></span>|<span data-ttu-id="b8206-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8206-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8206-111">none</span><span class="sxs-lookup"><span data-stu-id="b8206-111">none</span></span>|<span data-ttu-id="b8206-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b8206-112">0</span></span>|<span data-ttu-id="b8206-113">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="b8206-113">Default value, no intent.</span></span>|
|<span data-ttu-id="b8206-114">аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="b8206-114">appsInListCompliant</span></span>|<span data-ttu-id="b8206-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b8206-115">1</span></span>|<span data-ttu-id="b8206-116">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="b8206-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="b8206-117">аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="b8206-117">appsNotInListCompliant</span></span>|<span data-ttu-id="b8206-118">2</span><span class="sxs-lookup"><span data-stu-id="b8206-118">2</span></span>|<span data-ttu-id="b8206-119">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="b8206-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



