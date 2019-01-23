---
title: Тип перечисления groupPolicyConfigurationType
description: Тип настройки групповой политики
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 372a5bd5656510c43b388bac128cba4bc46c0988
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430706"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="0099f-103">Тип перечисления groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="0099f-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="0099f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0099f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0099f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0099f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0099f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0099f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0099f-107">Тип настройки групповой политики</span><span class="sxs-lookup"><span data-stu-id="0099f-107">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="0099f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0099f-108">Members</span></span>
|<span data-ttu-id="0099f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0099f-109">Member</span></span>|<span data-ttu-id="0099f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0099f-110">Value</span></span>|<span data-ttu-id="0099f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0099f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0099f-112">политика</span><span class="sxs-lookup"><span data-stu-id="0099f-112">policy</span></span>|<span data-ttu-id="0099f-113">0</span><span class="sxs-lookup"><span data-stu-id="0099f-113">0</span></span>|<span data-ttu-id="0099f-114">Тип политики не tattoo значение, которое означает, что значение было удалено, позволяя исходное значение конфигурации для использования.</span><span class="sxs-lookup"><span data-stu-id="0099f-114">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="0099f-115">Тип политики заменяет параметр конфигурации приложения, чтобы приложение всегда учитывать значение параметра.</span><span class="sxs-lookup"><span data-stu-id="0099f-115">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="0099f-116">Тип политики запрещает пользователю изменения значения через интерфейс пользователя.</span><span class="sxs-lookup"><span data-stu-id="0099f-116">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="0099f-117">preference</span><span class="sxs-lookup"><span data-stu-id="0099f-117">preference</span></span>|<span data-ttu-id="0099f-118">1</span><span class="sxs-lookup"><span data-stu-id="0099f-118">1</span></span>|<span data-ttu-id="0099f-119">Тип предпочтения tattoo значение, которое означает, что значение не удаляется из реестра.</span><span class="sxs-lookup"><span data-stu-id="0099f-119">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="0099f-120">Тип предпочтения заменяет настроен значение пользователя, не сохраняются предыдущего значения.</span><span class="sxs-lookup"><span data-stu-id="0099f-120">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="0099f-121">Тип предпочтения не запрещает пользователю изменения значения через интерфейс пользователя.</span><span class="sxs-lookup"><span data-stu-id="0099f-121">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|




