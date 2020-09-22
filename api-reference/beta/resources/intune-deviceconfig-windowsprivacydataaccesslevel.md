---
title: тип перечисления Виндовспривацидатаакцесслевел
description: Определите категорию уровня доступа к определенной конфиденциальной информации Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 420ad04f91331056245b042914985b1b7ca0c57a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061709"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="90b9a-103">тип перечисления Виндовспривацидатаакцесслевел</span><span class="sxs-lookup"><span data-stu-id="90b9a-103">windowsPrivacyDataAccessLevel enum type</span></span>

<span data-ttu-id="90b9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90b9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90b9a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90b9a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90b9a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90b9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90b9a-107">Определите категорию уровня доступа к определенной конфиденциальной информации Windows.</span><span class="sxs-lookup"><span data-stu-id="90b9a-107">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="90b9a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="90b9a-108">Members</span></span>
|<span data-ttu-id="90b9a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="90b9a-109">Member</span></span>|<span data-ttu-id="90b9a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="90b9a-110">Value</span></span>|<span data-ttu-id="90b9a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="90b9a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90b9a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="90b9a-112">notConfigured</span></span>|<span data-ttu-id="90b9a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="90b9a-113">0</span></span>|<span data-ttu-id="90b9a-114">Уровень доступа не указан, нет целей.</span><span class="sxs-lookup"><span data-stu-id="90b9a-114">No access level specified, no intents.</span></span> <span data-ttu-id="90b9a-115">Устройство может вести себя как в Усеринконтрол, так и Форцеаллов.</span><span class="sxs-lookup"><span data-stu-id="90b9a-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="90b9a-116">Это может зависеть от данных о конфиденциальности, а также версий Windows и других факторов.</span><span class="sxs-lookup"><span data-stu-id="90b9a-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="90b9a-117">форцеаллов</span><span class="sxs-lookup"><span data-stu-id="90b9a-117">forceAllow</span></span>|<span data-ttu-id="90b9a-118">1 </span><span class="sxs-lookup"><span data-stu-id="90b9a-118">1</span></span>|<span data-ttu-id="90b9a-119">Приложениям будет разрешен доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="90b9a-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="90b9a-120">форцедени</span><span class="sxs-lookup"><span data-stu-id="90b9a-120">forceDeny</span></span>|<span data-ttu-id="90b9a-121">2 </span><span class="sxs-lookup"><span data-stu-id="90b9a-121">2</span></span>|<span data-ttu-id="90b9a-122">Приложениям будет отказано в доступе к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="90b9a-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="90b9a-123">усеринконтрол</span><span class="sxs-lookup"><span data-stu-id="90b9a-123">userInControl</span></span>|<span data-ttu-id="90b9a-124">4</span><span class="sxs-lookup"><span data-stu-id="90b9a-124">3</span></span>|<span data-ttu-id="90b9a-125">Пользователи будут получать приглашение при попытке приложения получить доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="90b9a-125">Users will be prompted when apps try to access specified privacy data.</span></span>|






