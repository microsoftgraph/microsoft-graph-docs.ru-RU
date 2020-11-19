---
title: тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе
description: Возможные значения для Фиреваллпрешаредкэйенкодингмесод
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 79fcb89a8165cbea6d2132eda256c742231fd129
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303218"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="a7766-103">тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="a7766-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="a7766-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7766-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7766-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7766-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7766-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7766-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7766-107">Возможные значения для Фиреваллпрешаредкэйенкодингмесод</span><span class="sxs-lookup"><span data-stu-id="a7766-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="a7766-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a7766-108">Members</span></span>
|<span data-ttu-id="a7766-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a7766-109">Member</span></span>|<span data-ttu-id="a7766-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a7766-110">Value</span></span>|<span data-ttu-id="a7766-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a7766-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7766-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="a7766-112">deviceDefault</span></span>|<span data-ttu-id="a7766-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a7766-113">0</span></span>|<span data-ttu-id="a7766-114">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="a7766-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="a7766-115">Нет</span><span class="sxs-lookup"><span data-stu-id="a7766-115">none</span></span>|<span data-ttu-id="a7766-116">1,1</span><span class="sxs-lookup"><span data-stu-id="a7766-116">1</span></span>|<span data-ttu-id="a7766-117">Общий ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="a7766-117">Preshared key is not encoded.</span></span> <span data-ttu-id="a7766-118">Вместо этого он хранится в расширенном формате символов</span><span class="sxs-lookup"><span data-stu-id="a7766-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="a7766-119">utF8</span><span class="sxs-lookup"><span data-stu-id="a7766-119">utF8</span></span>|<span data-ttu-id="a7766-120">2</span><span class="sxs-lookup"><span data-stu-id="a7766-120">2</span></span>|<span data-ttu-id="a7766-121">Кодирование общего ключа с помощью UTF – 8</span><span class="sxs-lookup"><span data-stu-id="a7766-121">Encode the preshared key using UTF-8</span></span>|




