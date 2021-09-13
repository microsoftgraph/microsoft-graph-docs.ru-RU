---
title: тип enum policySetStatus
description: В этом переустановлении указывается состояние PolicySet.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22091444272c3e88648e1e14483ec58ce6f78873
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020324"
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
|проверка|1|Все элементы PolicySet теперь являются проверкой для соответствующих параметров рабочих нагрузок.|
|partialSuccess|2|После завершения процесса для всех элементов PolicySet, но есть сбои.|
|success|3|Развертываются все элементы PolicySet. Это не значит, что все развертывание успешно. |
|error|4 |Обработка PolicySet полностью провалилась.|
|notAssigned|5 |PolicySet/PolicySetItem не назначена ни одной группе.|



