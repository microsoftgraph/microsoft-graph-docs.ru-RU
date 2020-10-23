---
title: тип перечисления Виндовссмодеконфигуратион
description: Возможные варианты настройки S режима разблокировки
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7358f7067a868dd891b701f2d67c9abc5fbd422c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684857"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="9960d-103">тип перечисления Виндовссмодеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9960d-103">windowsSModeConfiguration enum type</span></span>

<span data-ttu-id="9960d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9960d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9960d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9960d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9960d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9960d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9960d-107">Возможные варианты настройки S режима разблокировки</span><span class="sxs-lookup"><span data-stu-id="9960d-107">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="9960d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9960d-108">Members</span></span>
|<span data-ttu-id="9960d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9960d-109">Member</span></span>|<span data-ttu-id="9960d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9960d-110">Value</span></span>|<span data-ttu-id="9960d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9960d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9960d-112">Ограничение</span><span class="sxs-lookup"><span data-stu-id="9960d-112">noRestriction</span></span>|<span data-ttu-id="9960d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="9960d-113">0</span></span>|<span data-ttu-id="9960d-114">Этот параметр удалит все ограничения для режима разблокировки S — значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="9960d-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="9960d-115">блок</span><span class="sxs-lookup"><span data-stu-id="9960d-115">block</span></span>|<span data-ttu-id="9960d-116">1,1</span><span class="sxs-lookup"><span data-stu-id="9960d-116">1</span></span>|<span data-ttu-id="9960d-117">Этот параметр блокирует возможность пользователя разблокировать устройство в режиме S</span><span class="sxs-lookup"><span data-stu-id="9960d-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="9960d-118">блокиру</span><span class="sxs-lookup"><span data-stu-id="9960d-118">unlock</span></span>|<span data-ttu-id="9960d-119">2</span><span class="sxs-lookup"><span data-stu-id="9960d-119">2</span></span>|<span data-ttu-id="9960d-120">Этот параметр позволяет разблокировать устройство в режиме S</span><span class="sxs-lookup"><span data-stu-id="9960d-120">This option will unlock the device from S mode</span></span>|





