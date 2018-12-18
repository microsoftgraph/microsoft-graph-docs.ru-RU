---
title: Тип перечисления firewallPreSharedKeyEncodingMethodType
description: Возможные значения для firewallPreSharedKeyEncodingMethod
author: tfitzmac
ms.openlocfilehash: 3ed2456f54bd27a3efa04d959edba48f7c100692
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324936"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="04e9a-103">Тип перечисления firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="04e9a-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="04e9a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="04e9a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04e9a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04e9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04e9a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="04e9a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04e9a-107">Возможные значения для firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="04e9a-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="04e9a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="04e9a-108">Members</span></span>
|<span data-ttu-id="04e9a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="04e9a-109">Member</span></span>|<span data-ttu-id="04e9a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="04e9a-110">Value</span></span>|<span data-ttu-id="04e9a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="04e9a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04e9a-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="04e9a-112">deviceDefault</span></span>|<span data-ttu-id="04e9a-113">0</span><span class="sxs-lookup"><span data-stu-id="04e9a-113">0</span></span>|<span data-ttu-id="04e9a-114">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="04e9a-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="04e9a-115">none</span><span class="sxs-lookup"><span data-stu-id="04e9a-115">none</span></span>|<span data-ttu-id="04e9a-116">1</span><span class="sxs-lookup"><span data-stu-id="04e9a-116">1</span></span>|<span data-ttu-id="04e9a-117">Предварительный ключ не кодируются.</span><span class="sxs-lookup"><span data-stu-id="04e9a-117">Preshared key is not encoded.</span></span> <span data-ttu-id="04e9a-118">Вместо этого он будет храниться в формате Юникода</span><span class="sxs-lookup"><span data-stu-id="04e9a-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="04e9a-119">utF8</span><span class="sxs-lookup"><span data-stu-id="04e9a-119">utF8</span></span>|<span data-ttu-id="04e9a-120">2</span><span class="sxs-lookup"><span data-stu-id="04e9a-120">2</span></span>|<span data-ttu-id="04e9a-121">Кодирование предварительный ключ, используя UTF-8</span><span class="sxs-lookup"><span data-stu-id="04e9a-121">Encode the preshared key using UTF-8</span></span>|





