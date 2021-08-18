---
title: тип enum policySetStatus
description: В этом переустановлении указывается состояние PolicySet.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a31849f4984edbabdda45e319df9a8cba5005cb76302f8b68dc414ef7a59b651
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54150187"
---
# <a name="policysetstatus-enum-type"></a>тип enum policySetStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этом переустановлении указывается состояние PolicySet.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Значение по умолчанию.|
|проверка|1 |Все элементы PolicySet теперь являются проверкой для соответствующих параметров рабочих нагрузок.|
|partialSuccess|2|После завершения процесса для всех элементов PolicySet, но есть сбои.|
|success|3 |Развертываются все элементы PolicySet. Это не значит, что все развертывание успешно. |
|error|4 |Обработка PolicySet полностью провалилась.|
|notAssigned|5 |PolicySet/PolicySetItem не назначена ни одной группе.|




