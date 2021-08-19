---
title: тип enum vppTokenState
description: Возможные состояния, связанные с маркером Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f7df4f078b91a6c42ac4718a30145e1e141d8436bd8932c25780ce678cf2366c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54172787"
---
# <a name="vpptokenstate-enum-type"></a>тип enum vppTokenState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные состояния, связанные с маркером Apple Volume Purchase Program.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние по умолчанию.|
|допустимо|1 |Маркер действителен.|
|истек срок действия|2|Срок действия маркера истек.|
|Недопустимый|3 |Маркер недействителен.|
|назначеноToExternalMDM|4 |Маркер управляется другой службой MDM.|
|duplicateLocationId|5 |Маркер связан с тем же расположением, что и другой маркер на учетной записи.|




